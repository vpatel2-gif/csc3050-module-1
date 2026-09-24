# HTTP Analysis

## Request 1
**Type:** Document
**Method:** GET
**URL:** https://www.walmart.com
**Status:** 200
**Headers:**
  Content-Type: text/html; charset=utf-8
  Cache-Control: max-age=0, no-cache, no-store
-**Duraction:** 2.20s 

## Request 2
**Type:** Script
**Method:** GET
**URL:** https://i5.walmartimages.com
**Status:** 200
**Headers:**
  Content-Length: 3251
  Content-Type: application/javascript
  Content-Control : public, max-age=30758400 
**Duraction:** 0ms

## Request 3
**Type:** Stylesheet
**Method:** GET
**URL:** https://i5.walmartimages.com
**Status:** 200
**Headers:**
  Content-Type: text/css
  Content-Encoding : br
**Duraction:** 1ms
## Analysis

**Frist Request**The document request was the slowest. It took longer to load, which could be because the website is a large commercial website with larger files. Network conditions, server processing, or the browser loading a large document could also cause the delay. The request method was GET, which is used to request data from a server. The status code was 200 (OK), meaning the server successfully processed the request and returned the resource. The Content-Type was text/html, which tells the browser that the response is an HTML document. The Cache-Control header provides instructions about caching. max-age=0 means the response is considered stale immediately and should be revalidated before being used from the cache.
**Second Request**The JavaScript request took 0 ms and also used GET with a 200 (OK) status. The Content-Length was 3251 bytes, which tells the browser the size of the response. The Content-Type was application/javascript, showing that the response was JavaScript. The Cache-Control header provides instructions about how long the response can remain fresh.
**Third Request**The stylesheet took 1 ms and used GET with a 200 (OK) status. The Content-Type was text/css, meaning the response was a CSS stylesheet. The Content-Encoding was br, which means Brotli compression was used to reduce the size of the transferred data.

One thing that surprised me was the Timing section in the Network tab. It shows the different steps of a request and how long each step takes, which helps explain the final loading time.


