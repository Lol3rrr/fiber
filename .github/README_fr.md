<p align="center">
  <a href="https://gofiber.io">
    <img alt="Fiber" height="125" src="https://github.com/gofiber/docs/blob/master/static/fiber_v2_logo.svg">
  </a>
  <br>
  <a href="https://github.com/gofiber/fiber/blob/master/.github/README.md">
    <img height="20px" src="https://github.com/gofiber/docs/blob/master/static/flags/en.svg">
  </a>
  <a href="https://github.com/gofiber/fiber/blob/master/.github/README_ru.md">
    <img height="20px" src="https://github.com/gofiber/docs/blob/master/static/flags/ru.svg">
  </a>
  <a href="https://github.com/gofiber/fiber/blob/master/.github/README_es.md">
    <img height="20px" src="https://github.com/gofiber/docs/blob/master/static/flags/es.svg">
  </a>
  <a href="https://github.com/gofiber/fiber/blob/master/.github/README_ja.md">
    <img height="20px" src="https://github.com/gofiber/docs/blob/master/static/flags/jp.svg">
  </a>
  <a href="https://github.com/gofiber/fiber/blob/master/.github/README_pt.md">
    <img height="20px" src="https://github.com/gofiber/docs/blob/master/static/flags/pt.svg">
  </a>
  <a href="https://github.com/gofiber/fiber/blob/master/.github/README_zh-CN.md">
    <img height="20px" src="https://github.com/gofiber/docs/blob/master/static/flags/ch.svg">
  </a>
  <a href="https://github.com/gofiber/fiber/blob/master/.github/README_de.md">
    <img height="20px" src="https://github.com/gofiber/docs/blob/master/static/flags/de.svg">
  </a>
  <a href="https://github.com/gofiber/fiber/blob/master/.github/README_nl.md">
    <img height="20px" src="https://github.com/gofiber/docs/blob/master/static/flags/nl.svg">
  </a>
  <a href="https://github.com/gofiber/fiber/blob/master/.github/README_ko.md">
    <img height="20px" src="https://github.com/gofiber/docs/blob/master/static/flags/ko.svg">
  </a>
  <!--<a href="https://github.com/gofiber/fiber/blob/master/.github/README_fr.md">
    <img height="20px" src="https://github.com/gofiber/docs/blob/master/static/flags/fr.svg">
  </a>-->
  <a href="https://github.com/gofiber/fiber/blob/master/.github/README_tr.md">
    <img height="20px" src="https://github.com/gofiber/docs/blob/master/static/flags/tr.svg">
  </a>
  <a href="https://github.com/gofiber/fiber/blob/master/.github/README_id.md">
    <img height="20px" src="https://github.com/gofiber/docs/blob/master/static/flags/id.svg">
  </a>
  <a href="https://github.com/gofiber/fiber/blob/master/.github/README_he.md">
    <img height="20px" src="https://github.com/gofiber/docs/blob/master/static/flags/il.svg">
  </a>
   <a href="https://github.com/gofiber/fiber/blob/master/.github/README_ar_SA.md">
     <img height="20px" src="https://github.com/gofiber/docs/blob/master/static/flags/sa.svg">
   </a>
  <br><br>
  <a href="https://github.com/gofiber/fiber/releases">
    <img src="https://img.shields.io/github/release/gofiber/fiber?style=flat-square">
  </a>
  <a href="https://docs.gofiber.io">
    <img src="https://img.shields.io/badge/api-docs-blue?style=flat-square">
  </a>
  <a href="https://pkg.go.dev/github.com/gofiber/fiber?tab=doc">
    <img src="https://img.shields.io/badge/go.dev-007d9c?logo=go&logoColor=white&style=flat-square">
  </a>
  <a href="https://goreportcard.com/report/github.com/gofiber/fiber">
    <img src="https://goreportcard.com/badge/github.com/gofiber/fiber?style=flat-square">
  </a>
  <a href="https://gocover.io/github.com/gofiber/fiber">
    <img src="https://img.shields.io/badge/coverage-91%25-brightgreen?style=flat-square">
  </a>
  <a href="https://github.com/gofiber/fiber/actions?query=workflow%3ATest">
    <img src="https://img.shields.io/github/workflow/status/gofiber/fiber/Test?label=tests&style=flat-square">
  </a>
  <a href="https://github.com/gofiber/fiber/actions?query=workflow%3AGosec">
    <img src="https://img.shields.io/github/workflow/status/gofiber/fiber/Gosec?label=gosec&style=flat-square">
  </a>
  <a href="https://gofiber.io/discord">
    <img src="https://img.shields.io/badge/discord-join%20channel-7289DA?style=flat-square">
  </a>
</p>
<p align="center">
  <b>Fiber</b> est un framework web  inspiré d' <a href="https://github.com/expressjs/express">Express</a>. Il se base sur <a href="https://github.com/valyala/fasthttp">Fasthttp</a>, l'implémentation HTTP de <a href="https://golang.org/doc/">Go</a> <b>la plus rapide</b>. Conçu pour <b>faciliter</b> les choses pour des développements <b>rapides</b>, Fiber garde à l'esprit <b>l'absence d'allocations mémoires</b>, ainsi que les <b>performances</b>.
</p>

## ⚡️ Quickstart

```go
package main

import "github.com/gofiber/fiber"

func main() {
  app := fiber.New()

  app.Get("/", func(c *fiber.Ctx) {
    c.Send("Hello, World!")
  })

  app.Listen(3000)
}
```

## ⚙️ Installation

Premièrement, [téléchargez](https://golang.org/dl/) et installez Go. Version `1.11` ou supérieur requise.

L'installation est ensuite lancée via la commande  [`go get`](https://golang.org/cmd/go/#hdr-Add_dependencies_to_current_module_and_install_them):

```bash
go get -u github.com/gofiber/fiber/...
```

## 🤖 Benchmarks

Ces tests sont effectués par [TechEmpower](https://github.com/TechEmpower/FrameworkBenchmarks) et [Go Web](https://github.com/smallnest/go-web-framework-benchmark). Si vous voulez voir tous les résultats, n'hésitez pas à consulter notre [Wiki](https://docs.gofiber.io/benchmarks).

<p float="left" align="middle">
  <img src="https://github.com/gofiber/docs/blob/master/.gitbook/assets//benchmark-pipeline.png" width="49%">
  <img src="https://github.com/gofiber/docs/blob/master/.gitbook/assets//benchmark_alloc.png" width="49%">
</p>

## 🎯 Features

-  [Routing](https://docs.gofiber.io/routing) robuste
- Serve [static files](https://docs.gofiber.io/application#static)
- [Performances](https://docs.gofiber.io/benchmarks) extrêmes
- [Faible empreinte mémoire](https://docs.gofiber.io/benchmarks)
- [API endpoints](https://docs.gofiber.io/context)
- Middleware & [Next](https://docs.gofiber.io/context#next) support
- Programmation côté serveur [rapide](https://dev.to/koddr/welcome-to-fiber-an-express-js-styled-fastest-web-framework-written-with-on-golang-497)
- [Template engines](https://docs.gofiber.io/middleware#template)
- [WebSocket support](https://docs.gofiber.io/middleware#websocket)
- [Rate Limiter](https://docs.gofiber.io/middleware#limiter)
- Available in [12 languages](https://docs.gofiber.io/)
- Et plus encore, [explorez Fiber](https://docs.gofiber.io/)

## 💡 Philosophie

Les nouveaux gophers qui passent de [Node.js](https://nodejs.org/en/about/) à [Go](https://golang.org/doc/) sont confrontés à une courbe d'apprentissage, avant de pouvoir construire leurs applications web et microservices. Fiber, en tant que **framework web**, a été mis au point avec en tête l'idée de **minimalisme**, tout en suivant l'**UNIX way**, afin que les nouveaux gophers puissent rapidement entrer dans le monde de Go, avec un accueil chaleureux, de confiance.

Fiber est **inspiré** par Express, le framework web le plus populaire d'Internet. Nous avons combiné la **facilité** d'Express, et la **performance brute** de Go. Si vous avez déja développé une application web en Node.js (_en utilisant Express ou équivalent_), alors de nombreuses méthodes et principes vous sembleront **familiers**.

## 👀 Exemples

Ci-dessous quelques exemples courants. Si vous voulez voir plus d'exemples, rendez-vous sur notre ["Recipes repository"](https://github.com/gofiber/recipes) ou visitez notre [documentation API](https://docs.gofiber.io).

### Routing

📖 [Routing](https://docs.gofiber.io/#basic-routing)  


```go
func main() {
  app := fiber.New()

  // GET /john
  app.Get("/:name", func(c *fiber.Ctx) {
    fmt.Printf("Hello %s!", c.Params("name"))
    // => Hello john!
  })

  // GET /john
  app.Get("/:name/:age?", func(c *fiber.Ctx) {
    fmt.Printf("Name: %s, Age: %s", c.Params("name"), c.Params("age"))
    // => Name: john, Age:
  })

  // GET /api/register
  app.Get("/api/*", func(c *fiber.Ctx) {
    fmt.Printf("/api/%s", c.Params("*"))
    // => /api/register
  })

  app.Listen(3000)
}
```

### Serve static files

📖 [Static](https://docs.gofiber.io/application#static)  

```go
func main() {
  app := fiber.New()

  app.Static("/", "/public")
  // => http://localhost:3000/js/script.js
  // => http://localhost:3000/css/style.css

  app.Static("/prefix", "/public")
  // => http://localhost:3000/prefix/js/script.js
  // => http://localhost:3000/prefix/css/style.css

  app.Static("*", "/public/index.html")
  // => http://localhost:3000/any/path/shows/index/html

  app.Listen(3000)
}
```

### Middleware & Next

📖 [Middleware](https://docs.gofiber.io/routing#middleware)  
📖 [Next](https://docs.gofiber.io/context#next)  

```go
func main() {
  app := fiber.New()

  // Match any route
  app.Use(func(c *fiber.Ctx) {
    fmt.Println("First middleware")
    c.Next()
  })

  // Match all routes starting with /api
  app.Use("/api", func(c *fiber.Ctx) {
    fmt.Println("Second middleware")
    c.Next()
  })

  // GET /api/register
  app.Get("/api/list", func(c *fiber.Ctx) {
    fmt.Println("Last middleware")
    c.Send("Hello, World!")
  })

  app.Listen(3000)
}
```

<details>
  <summary>📚 Show more code examples</summary>

### Template engines

📖 [Settings](https://docs.gofiber.io/application#settings)  
📖 [Render](https://docs.gofiber.io/context#render)  
📖 [Template](https://docs.gofiber.io/middleware#template)  

Fiber supports the default [Go template engine](https://golang.org/pkg/html/template/)

But if you want to use another template engine like [amber](https://github.com/eknkc/amber), [handlebars](https://github.com/aymerick/raymond), [mustache](https://github.com/cbroglie/mustache) or [pug](https://github.com/Joker/jade).

You can use our [Template Middleware](https://docs.gofiber.io/middleware#template).

```go
import (
  "github.com/gofiber/fiber"
  "github.com/gofiber/template"
)

func main() {
  // You can setup template engine before initiation app:
  app := fiber.New(&fiber.Settings{
    TemplateEngine:    template.Mustache(),
    TemplateFolder:    "./views",
    TemplateExtension: ".tmpl",
  })

  // OR after initiation app at any convenient location:
  app.Settings.TemplateEngine = template.Mustache()
  app.Settings.TemplateFolder = "./views"
  app.Settings.TemplateExtension = ".tmpl"

  // And now, you can call template `./views/home.tmpl` like this:
  app.Get("/", func(c *fiber.Ctx) {
    c.Render("home", fiber.Map{
      "title": "Homepage",
      "year":  1999,
    })
  })

  // ...
}
```

### Grouping routes into chains

📖 [Group](https://docs.gofiber.io/application#group)  

```go
func main() {
  app := fiber.New()

  // Root API route
  api := app.Group("/api", cors())  // /api

  // API v1 routes
  v1 := api.Group("/v1", mysql())   // /api/v1
  v1.Get("/list", handler)          // /api/v1/list
  v1.Get("/user", handler)          // /api/v1/user

  // API v2 routes
  v2 := api.Group("/v2", mongodb()) // /api/v2
  v2.Get("/list", handler)          // /api/v2/list
  v2.Get("/user", handler)          // /api/v2/user

  // ...
}
```

### Middleware logger

📖 [Logger](https://docs.gofiber.io/middleware#logger)  

```go
import (
    "github.com/gofiber/fiber"
    "github.com/gofiber/logger"
)

func main() {
    app := fiber.New()

    // Optional logger config
    config := logger.Config{
      Format:     "${time} - ${method} ${path}\n",
      TimeFormat: "Mon, 2 Jan 2006 15:04:05 MST",
    }

    // Logger with config
    app.Use(logger.New(config))

    app.Listen(3000)
}
```

### Cross-Origin Resource Sharing (CORS)

📖 [CORS](https://docs.gofiber.io/middleware#cors)  

```go
import (
    "github.com/gofiber/fiber"
    "github.com/gofiber/cors"
)

func main() {
    app := fiber.New()

    // CORS with default config
    app.Use(cors.New())

    app.Listen(3000)
}
```

Check CORS by passing any domain in `Origin` header:

```bash
curl -H "Origin: http://example.com" --verbose http://localhost:3000
```

### Custom 404 response

📖 [HTTP Methods](https://docs.gofiber.io/application#http-methods)  

```go
func main() {
  app := fiber.New()

  app.Static("/public")

  app.Get("/demo", func(c *fiber.Ctx) {
    c.Send("This is a demo!")
  })

  app.Post("/register", func(c *fiber.Ctx) {
    c.Send("Welcome!")
  })

  // Last middleware to match anything
  app.Use(func(c *fiber.Ctx) {
    c.SendStatus(404) 
    // => 404 "Not Found"
  })

  app.Listen(3000)
}
```

### JSON Response

📖 [JSON](https://docs.gofiber.io/context#json)  

```go
type User struct {
  Name string `json:"name"`
  Age  int    `json:"age"`
}

func main() {
  app := fiber.New()

  app.Get("/user", func(c *fiber.Ctx) {
    c.JSON(&User{"John", 20})
    // => {"name":"John", "age":20}
  })

  app.Get("/json", func(c *fiber.Ctx) {
    c.JSON(fiber.Map{
      "success": true,
      "message": "Hi John!",
    })
    // => {"success":true, "message":"Hi John!"}
  })

  app.Listen(3000)
}
```

### WebSocket Upgrade

📖 [Websocket](https://docs.gofiber.io/middleware#websocket)  

```go
import (
    "github.com/gofiber/fiber"
    "github.com/gofiber/websocket"
)

func main() {
  app := fiber.New()

  app.Get("/ws", websocket.New(func(c *websocket.Conn) {
    for {
      mt, msg, err := c.ReadMessage()
      if err != nil {
        log.Println("read:", err)
        break
      }
      log.Printf("recv: %s", msg)
      err = c.WriteMessage(mt, msg)
      if err != nil {
        log.Println("write:", err)
        break
      }
    }
  }))

  app.Listen(3000)
  // ws://localhost:3000/ws
}
```

### Recover middleware

📖 [Recover](https://docs.gofiber.io/middleware#recover)  

```go
import (
    "github.com/gofiber/fiber"
    "github.com/gofiber/recover"
)

func main() {
  app := fiber.New()

  // Optional recover config
  config := recover.Config{
    Handler: func(c *fiber.Ctx, err error) {
			c.SendString(err.Error())
			c.SendStatus(500)
		},
  }

  // Logger with custom config
  app.Use(recover.New(config))

  app.Listen(3000)
}
```
</details>

## 🧬 Official Middlewares

For an more _maintainable_ middleware _ecosystem_, we've put official [middlewares](https://docs.gofiber.io/middleware) into separate repositories:

- [gofiber/compression](https://github.com/gofiber/compression)
- [gofiber/basicauth](https://github.com/gofiber/basicauth)
- [gofiber/requestid](https://github.com/gofiber/requestid)
- [gofiber/websocket](https://github.com/gofiber/websocket)
- [gofiber/keyauth](https://github.com/gofiber/keyauth)
- [gofiber/rewrite](https://github.com/gofiber/rewrite)
- [gofiber/recover](https://github.com/gofiber/recover)
- [gofiber/limiter](https://github.com/gofiber/limiter)
- [gofiber/session](https://github.com/gofiber/session)
- [gofiber/adaptor](https://github.com/gofiber/adaptor)
- [gofiber/logger](https://github.com/gofiber/logger)
- [gofiber/helmet](https://github.com/gofiber/helmet)
- [gofiber/embed](https://github.com/gofiber/embed)
- [gofiber/pprof](https://github.com/gofiber/pprof)
- [gofiber/cors](https://github.com/gofiber/cors)
- [gofiber/csrf](https://github.com/gofiber/csrf)
- [gofiber/jwt](https://github.com/gofiber/jwt)

## 🌱 Third Party Middlewares

This is a list of middlewares that are created by the Fiber community, please create a PR if you want to see yours!
- [arsmn/fiber-swagger](https://github.com/arsmn/fiber-swagger)
- [arsmn/fiber-casbin](https://github.com/arsmn/fiber-casbin)
- [arsmn/fiber-introspect](https://github.com/arsmn/fiber-introspect)
- [shareed2k/fiber_tracing](https://github.com/shareed2k/fiber_tracing)
- [shareed2k/fiber_limiter](https://github.com/shareed2k/fiber_limiter)
- [thomasvvugt/fiber-boilerplate](https://github.com/thomasvvugt/fiber-boilerplate)
- [arsmn/gqlgen](https://github.com/arsmn/gqlgen)

## 💬 Media

- [Welcome to Fiber — an Express.js styled web framework written in Go with ❤️](https://dev.to/koddr/welcome-to-fiber-an-express-js-styled-fastest-web-framework-written-with-on-golang-497) — _03 Feb 2020_
- [Fiber released v1.7! 🎉 What's new and is it still fast, flexible and friendly?](https://dev.to/koddr/fiber-v2-is-out-now-what-s-new-and-is-he-still-fast-flexible-and-friendly-3ipf) — _21 Feb 2020_
- [🚀 Fiber v1.8. What's new, updated and re-thinked?](https://dev.to/koddr/fiber-v1-8-what-s-new-updated-and-re-thinked-339h) — _03 Mar 2020_
- [Is switching from Express to Fiber worth it? 🤔](https://dev.to/koddr/are-sure-what-your-lovely-web-framework-running-so-fast-2jl1) — _01 Apr 2020_
- [Creating Fast APIs In Go Using Fiber](https://dev.to/jozsefsallai/creating-fast-apis-in-go-using-fiber-59m9) — _07 Apr 2020_
- [Building a Basic REST API in Go using Fiber](https://tutorialedge.net/golang/basic-rest-api-go-fiber/) - _23 Apr 2020_
- [📺 Building a REST API using GORM and Fiber](https://youtu.be/Iq2qT0fRhAA) - _25 Apr 2020_
- [🌎 Create a travel list app with Go, Fiber, Angular, MongoDB and Google Cloud Secret Manager](https://blog.yongweilun.me/create-a-travel-list-app-with-go-fiber-angular-mongodb-and-google-cloud-secret-manager-ck9fgxy0p061pcss1xt1ubu8t) - _25 Apr 2020_
- [Fiber v1.9.6 🔥 How to improve performance by 817% and stay fast, flexible and friendly?](https://dev.to/koddr/fiber-v1-9-5-how-to-improve-performance-by-817-and-stay-fast-flexible-and-friendly-2dp6) - _12 May 2020_

## 👍 Contribuer

Si vous voulez nous remercier et/ou soutenir le développement actif de `Fiber`:

1. Ajoutez une [GitHub Star](https://github.com/gofiber/fiber/stargazers) à ce projet.
2. Twittez à propos de ce projet [sur votre Twitter](https://twitter.com/intent/tweet?text=Fiber%20is%20an%20Express%20inspired%20%23web%20%23framework%20built%20on%20top%20of%20Fasthttp%2C%20the%20fastest%20HTTP%20engine%20for%20%23Go.%20Designed%20to%20ease%20things%20up%20for%20%23fast%20development%20with%20zero%20memory%20allocation%20and%20%23performance%20in%20mind%20%F0%9F%9A%80%20https%3A%2F%2Fgithub.com%2Fgofiber%2Ffiber).
3. Ecrivez un article (review, tutorial) sur [Medium](https://medium.com/), [Dev.to](https://dev.to/), ou encore un blog personnel.
4. Help us to translate our API Documentation via [Crowdin](https://crowdin.com/project/gofiber) [![Crowdin](https://badges.crowdin.net/gofiber/localized.svg)](https://crowdin.com/project/gofiber)
5. Support the project by donating a [cup of coffee](https://buymeacoff.ee/fenny).

## ☕ Supporters

Fiber is an open source project that runs on donations to pay the bills e.g. our domain name, gitbook, netlify and serverless hosting. If you want to support Fiber, you can ☕ [**buy a coffee here**](https://buymeacoff.ee/fenny).

|                                                             | User                                            | Donation |
| :---------------------------------------------------------- | :---------------------------------------------- | :------- |
| ![](https://avatars.githubusercontent.com/u/59947262?s=25 ) | [@thomasvvugt](https://github.com/thomasvvugt)  | ☕ x 5    |
| ![](https://avatars.githubusercontent.com/u/1094221?s=25 )  | [@ekaputra07](https://github.com/ekaputra07)    | ☕ x 5    |
| ![](https://avatars.githubusercontent.com/u/186637?s=25 )   | [@candidosales](https://github.com/candidosales)| ☕ x 5    |
| ![](https://avatars.githubusercontent.com/u/635852?s=25 )   | [@bihe](https://github.com/bihe)                | ☕ x 3    |
| ![](https://avatars.githubusercontent.com/u/307334?s=25 )   | [@justdave](https://github.com/justdave)        | ☕ x 3    |
| ![](https://avatars.githubusercontent.com/u/11155743?s=25 ) | [@koddr](https://github.com/koddr)              | ☕ x 1    |
| ![](https://avatars.githubusercontent.com/u/29042462?s=25 ) | [@lapolinar](https://github.com/lapolinar)      | ☕ x 1    |
| ![](https://avatars.githubusercontent.com/u/2978730?s=25 )  | [@diegowifi](https://github.com/diegowifi)      | ☕ x 1    |
| ![](https://avatars.githubusercontent.com/u/44171355?s=25 ) | [@ssimk0](https://github.com/ssimk0)            | ☕ x 1    |
| ![](https://avatars.githubusercontent.com/u/5638101?s=25 )  | [@raymayemir](https://github.com/raymayemir)    | ☕ x 1    |
| ![](https://avatars.githubusercontent.com/u/619996?s=25 )   | [@melkorm](https://github.com/melkorm)          | ☕ x 1    |
| ![](https://avatars.githubusercontent.com/u/31022056?s=25 ) | [@marvinjwendt](https://github.com/thomasvvugt) | ☕ x 1    |
| ![](https://avatars.githubusercontent.com/u/31921460?s=25 ) | [@toishy](https://github.com/toishy)            | ☕ x 1    |

## ‎‍💻 Code Contributors

<img src="https://opencollective.com/fiber/contributors.svg?width=890&button=false" alt="Code Contributors" style="max-width:100%;">

## ⚠️ License

Copyright (c) 2019-present [Fenny](https://github.com/fenny) and [Contributors](https://github.com/gofiber/fiber/graphs/contributors). `Fiber` is free and open-source software licensed under the [MIT License](https://github.com/gofiber/fiber/blob/master/LICENSE). Official logo was created by [Vic Shóstak](https://github.com/koddr) and distributed under [Creative Commons](https://creativecommons.org/licenses/by-sa/4.0/) license (CC BY-SA 4.0 International).

**Third-party library licenses**
- [FastHTTP](https://github.com/valyala/fasthttp/blob/master/LICENSE)
- [Schema](https://github.com/gorilla/schema/blob/master/LICENSE)
- [bytebufferpool](https://github.com/valyala/bytebufferpool/blob/master/LICENSE)
