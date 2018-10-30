# bs-next-alt

## Introduction

Bucklescript + ReasonReact binding for [nextjs 7](https://github.com/zeit/next.js/) components. 
This is a quick fork of [bs-next](https://github.com/ulrikstrid/bs-next).  It wasn't building for me
so I needed to figure out why.  I am still trying to figure out why and when I do I will push there, 
but for now, this seems to work for me.
 
See [bs-ant-design](https://github.com/thangngoc89/bs-ant-design) repo for credit on binding pattern. 

## Installation
```
npm install --save bs-next-alt
```

* Add `bs-next-alt` to `bs-dependencies` in `bsconfig.json`.


## Usage
```
let component = ReasonReact.statelessComponent("Index");

let make = (_children) => {
  ...component,
  render: (_self) =>
    <div>
      <Next.Head>
        <title> (ReasonReact.stringToElement("My Page Title")) </title>
      </Next.Head>

      <Next.Link href="/about">
        <a> (ReasonReact.stringToElement("About")) </a>
      </Next.Link>
    </div>
}
```

## Components
link, head, error

## Contributions

All contributions are welcomed.  I intend to merge and release anything you pull request quickly.

## LICENSE

MIT
