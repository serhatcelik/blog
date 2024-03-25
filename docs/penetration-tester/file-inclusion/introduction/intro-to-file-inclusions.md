---
icon: material/circle-small
---

# Intro to File Inclusions

## PHP

```php
if (isset($_GET['language'])) {
    include($_GET['language']);
}
```

| Function | Read Content | Execute | Remote URL |
|:---|:---:|:---:|:---:|
| `include()` | X | X | X |
| `require()` | X | X ||
| `file_get_contents()` | X || X |
| `fopen()` | X |||

## NodeJS

```javascript
if(req.query.language) {
    fs.readFile(path.join(__dirname, req.query.language), function (err, data) {
        res.write(data);
    });
}
```

| Function | Read Content | Execute | Remote URL |
|:---|:---:|:---:|:---:|
| `fs.readFile()` | X |||
| `fs.sendFile()` | X |||
| `res.render()` | X | X ||

## Java

```jsp
<c:if test="${not empty param.language}">
    <jsp:include file="<%= request.getParameter('language') %>" />
</c:if>
```

| Function | Read Content | Execute | Remote URL |
|:---|:---:|:---:|:---:|
| `include` | X |||
| `import` | X | X | X |

## .NET

```cs
@if (!string.IsNullOrEmpty(HttpContext.Request.Query['language'])) {
    <% Response.WriteFile("<% HttpContext.Request.Query['language'] %>"); %>
}
```

| Function | Read Content | Execute | Remote URL |
|:---|:---:|:---:|:---:|
| `@Html.Partial()` | X |||
| `@Html.RemotePartial()` | X || X |
| `Response.WriteFile()` | X |||
| `include` | X | X | X |
