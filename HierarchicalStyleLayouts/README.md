### Hierarchical Style Layouts

- First Have A Template 
- Create A Layout Folder or File
- The Layout file we never be returned directly
- Now we our htm to share the same layout
- insert an extra dependency

```pom.xml
 <dependency>
            <groupId>nz.net.ultraq.thymeleaf</groupId>
            <artifactId>thymeleaf-layout-dialect</artifactId>
</dependency>
```

- Add this to your thymeleaf page html tag attribute
`
xmlns:th="http://thymeleaf.org" xmlns:layout="http://www.ultraq.net.nz/thymeleaf/la"
`

- Create the Placeholder section in the layout file and assign it a key
  layout:fragment="main-content"

- Head to your decorate file (index)
call the exact placeholder key created in the layout file 
to connect both file prepend to your html tag attribute 
`layout:decorate="layout"` or use fragment expression
`layout:decorate="~{layout}"`
Both are refering to layout.html