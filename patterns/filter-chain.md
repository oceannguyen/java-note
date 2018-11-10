# Filter Chain pattern

> A ```FilterChain``` is an object provided by the servlet container to the developer giving a view into the invocation chain of a filtered request for a resource. Filters use the FilterChain to invoke the next filter in the chain, or if the calling filter is the last filter in the chain, to invoke the resource at the end of the chain.

## What are Filter?

> Servlet filters are implementation of the chain of responsibility pattern.

```Filters``` are used to ```intercept and process requests``` before they are sent to servlets (in case of request).
**OR**
```Filters``` are used to ```intercept and process a response``` before they are sent back to client by a servlet.

## Why they are used?

- Filters can perform security checks.

- Compress the response stream.

- Create a different response.

## What does ```doFilter()``` do?

> The ```doFilter()``` is called ```every time``` the container determines that the filter should be applied to a page.

It takes ```three arguments```

- ```ServletRequest```

- ```ServlerResponse```

- ```FilterChain```

All the ```functionality that your filter supposed to do``` is implemented inside ```doFilter()``` method.