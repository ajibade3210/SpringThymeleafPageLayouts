## ThymeLeaf Page Layout

Usually websites share common page components like the header, footer, menu and possibly many more. These page components can be used by the same or different layouts.

There are two main styles of organizing layouts in thymeleaf

### - Include Style:

The include-style layouts are pretty simple to understand and implement and in fact they offer flexibility in developing views, which is their biggest advantage. The main disadvantage of this solution, though, is that some code duplication is introduced so modifying the layout of a large number of views in big applications can become a bit cumbersome.

![Logo](https://i.imgur.com/mUJUUqn.jpg)

### - Hierarchical-style layouts:

In hierarchical style, the templates are usually created with a parent-child relation, from the more general part (layout) to the most specific ones (subviews; e.g. page content). Each component of the template may be included dynamically based on the inclusion and substitution of template fragments. In Thymeleaf this can be done using Thymeleaf Layout Dialect.

The main advantages of this solution are the reuse of atomic portions of the view and modular design, whereas the main disadvantage is that much more configuration is needed in order to use them, so the complexity of the views is bigger than with Include Style Layouts which are more “natural” to use.

![Logo](https://i.imgur.com/mUJUUqn.jpg)
