---
path: test
date: 2020-04-23T04:07:53.805Z
title: Test title
description: This is about testing Netlify to see what its like
---
# So what is this about

## About testing of course.

![V60 coffee](/assets/andrew-welch-77146-unsplash.jpg "V60 coffee")

How [about a link](https://www.thomaswang.io/blog/how-to-make-a-fully-featured-dev-blog-in-under-10-minutes/)

* Number one
* two
* three
* four

1. four
2. three
3. two
4. one

> This is the quote of the day

```
import React from "react"
```

```
import { Link } from "gatsby"
```

```
import styled from "styled-components"
```

```

```

```
import { rhythm, scale } from "../utils/typography"
```

```

```

```
class Layout extends React.Component {
```

```
  render() {
```

```
    const { location, title, children } = this.props
```

```
    const rootPath = `${__PATH_PREFIX__}/`
```

```
    const blogPath = `${__PATH_PREFIX__}/blog/`
```

```
    let header
```

```

```

```
    if (location.pathname === rootPath || location.pathname === blogPath) {
```

```
      header = (
```

```
        <h1
```

```
          style={{
```

```
            ...scale(1.5),
```

```
            marginBottom: rhythm(1.5),
```

```
            marginTop: 0,
```

```
          }}
```

```
        >
```

```
          <Link
```

```
            style={{
```

```
              boxShadow: `none`,
```

```
              textDecoration: `none`,
```

```
              color: `inherit`,
```

```
            }}
```

```
            to={location.pathname === blogPath ? `/blog/` : `/`}
```

```
          >
```

```
            {title}
```

```
          </Link>
```

```
        </h1>
```

```
      )
```

```
    } else {
```

```
      header = (
```

```
        <h3
```

```
          style={{
```

```
            fontFamily: `Montserrat, sans-serif`,
```

```
            marginTop: 0,
```

```
          }}
```

```
        >
```

```
          <Link
```

```
            style={{
```

```
              boxShadow: `none`,
```

```
              textDecoration: `none`,
```

```
              color: `inherit`,
```

```
            }}
```

```
            to={`/blog/`}
```

```
          >
```

```
            {title}
```

```
          </Link>
```

```
        </h3>
```

```
      )
```

```
    }
```

```
    return (
```

```
      <Wrapper>
```

```
        <div
```

```
          style={{
```

```
            marginLeft: `auto`,
```

```
            marginRight: `auto`,
```

```
            maxWidth: rhythm(24),
```

```
            padding: `${rhythm(1.5)} ${rhythm(3 / 4)}`,
```

```
          }}
```

```
        >
```

```
          <header>{header}</header>
```

```
          <main>{children}</main>
```

```
        </div>
```

```
        <Footer>
```

```
          © {new Date().getFullYear()}, Built with
```

```
          {` `}
```

```
          <a href="https://www.gatsbyjs.org">Gatsby</a>
```

```
        </Footer>
```

```
      </Wrapper>
```

```
    )
```

```
  }
```

```
}
```

```

```

```
const Wrapper = styled.div`
```

```
  min-height: 100vh;
```

```
`
```

```

```

```
const Footer = styled.footer`
```

```
  text-align: center;
```

```
  margin: 24px;
```

```
`
```

```

```





`import React from "react"`

`import { Link } from "gatsby"`

`import styled from "styled-components"`

``

`import { rhythm, scale } from "../utils/typography"`

``

`class Layout extends React.Component {`

`  render() {`

`    const { location, title, children } = this.props`

``    const rootPath = `${__PATH_PREFIX__}/` ``

``    const blogPath = `${__PATH_PREFIX__}/blog/` ``

`    let header`

``

`    if (location.pathname === rootPath || location.pathname === blogPath) {`

`      header = (`

`        <h1`

`          style={{`

`            ...scale(1.5),`

`            marginBottom: rhythm(1.5),`

`            marginTop: 0,`

`          }}`

`        >`

`          <Link`

`            style={{`

``              boxShadow: `none`,``

``              textDecoration: `none`,``

``              color: `inherit`,``

`            }}`

``            to={location.pathname === blogPath ? `/blog/` : `/`}``

`          >`

`            {title}`

`          </Link>`

`        </h1>`

`      )`

`    } else {`

`      header = (`

`        <h3`

`          style={{`

``            fontFamily: `Montserrat, sans-serif`,``

`            marginTop: 0,`

`          }}`

`        >`

`          <Link`

`            style={{`

``              boxShadow: `none`,``

``              textDecoration: `none`,``

``              color: `inherit`,``

`            }}`

``            to={`/blog/`}``

`          >`

`            {title}`

`          </Link>`

`        </h3>`

`      )`

`    }`

`    return (`

`      <Wrapper>`

`        <div`

`          style={{`

``            marginLeft: `auto`,``

``            marginRight: `auto`,``

`            maxWidth: rhythm(24),`

``            padding: `${rhythm(1.5)} ${rhythm(3 / 4)}`,``

`          }}`

`        >`

`          <header>{header}</header>`

`          <main>{children}</main>`

`        </div>`

`        <Footer>`

`          © {new Date().getFullYear()}, Built with`

``          {` `}``

`          <a href="https://www.gatsbyjs.org">Gatsby</a>`

`        </Footer>`

`      </Wrapper>`

`    )`

`  }`

`}`

``

``const Wrapper = styled.div` ``

`  min-height: 100vh;`

`` ` ``

``

``const Footer = styled.footer` ``

`  text-align: center;`

`  margin: 24px;`

`` ` ``

``

`export default Layout`
