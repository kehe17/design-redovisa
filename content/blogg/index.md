---
views:
    main:
        template: anax/v2/article/default
        data:
            class: blog

    byline: false
    block-about: false
    article-toc: false

    blog-list:
        region: main
        template: anax/v2/blog-list/default
        sort: 2
        data:
            dateFormat: M j, Y, g:ia
            meta: 
                type: toc
                orderby: publishTime
                orderorder: desc

    blog-toc:
        region: sidebar-right
        template: anax/v2/blog-toc/default
        sort: 2
        data:
            meta: 
                type: copy
                view: blog-list

---
Picture of the Day
===========================

Blog to try out Cimage for kmom05. It's just cat pictures, because really, isn't that what all blogs are?
