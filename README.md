你好！
很冒昧用这样的方式来和你沟通，如有打扰请忽略我的提交哈。我是光年实验室（gnlab.com）的HR，在招Golang开发工程师，我们是一个技术型团队，技术氛围非常好。全职和兼职都可以，不过最好是全职，工作地点杭州。
我们公司是做流量增长的，Golang负责开发SAAS平台的应用，我们做的很多应用是全新的，工作非常有挑战也很有意思，是国内很多大厂的顾问。
如果有兴趣的话加我微信：13515810775  ，也可以访问 https://gnlab.com/，联系客服转发给HR。
<h1 align="center">
  <br>
  <a href="https://github.com/sensepost/objection">
    <img src="images/gowitness-logo.png" alt="objection"></a>
  <br>
  <br>
</h1>

<h4 align="center">A golang, web screenshot utility using Chrome Headless.</h4>
<br>

## introduction
`gowitness` is a website screenshot utility written in Golang, that uses Chrome Headless to generate screenshots of web interfaces using the command line. Both Linux and macOS is supported, with Windows support 'partially working'.

Inspiration for `gowitness` comes from [Eyewitness](https://github.com/ChrisTruncer/EyeWitness). If you are looking for something with lots of extra features, be sure to check it out along with these [other](https://github.com/afxdub/http-screenshot-html) [projects](https://github.com/breenmachine/httpscreenshot).

## installation
All you would need is an installation of the latest Google Chrome or Chromium and `gowitness` itself. Binaries are available for download from the [releases](https://github.com/sensepost/gowitness/releases) page as part of tagged releases.

To build `gowitness` from source, follow the following steps:

* Ensure you have [dep](https://github.com/golang/dep) installed (`go get -v -u github.com/golang/dep/cmd/dep`)
* Clone this repository to your `$GOPATH`'s `src/` directory so that it is in `sensepost/gowitness`
* Run `dep ensure` to resolve dependencies
* Use the `go` build tools, or run `make` to build the binaries in the `build/` directory

## usage
```
~ » gowitness -h
A commandline web screenshot and information gathering tool.

Usage:
  gowitness [command]

Available Commands:
  file        Screenshot URLs sourced from a file
  generate    Generate an HTML report from a database file
  help        Help about any command
  scan        Scan a CIDR range and take screenshots along the way
  single      Take a screenshot of a single URL
  version     Prints the version of gowitness

Flags:
      --chrome-timeout int   Time in seconds to wait for Google Chrome to finish a screenshot (default 90)
      --config string        config file (default is $HOME/.gowitness.yaml)
  -D, --db string            Destination for the gowitness database (default "gowitness.db")
  -d, --destination string   Destination directory for screenshots (default ".")
  -h, --help                 help for gowitness
      --log-format string    specify output (text or json) (default "text")
      --log-level string     one of debug, info, warn, error, or fatal (default "info")
  -R, --resolution string    screenshot resolution (default "1440,900")
  -T, --timeout int          Time in seconds to wait for a HTTP connection (default 3)

Use "gowitness [command] --help" for more information about a command.
```

## license

gowtiness is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/) Permissions beyond the scope of this license may be available at http://sensepost.com/contact/.
