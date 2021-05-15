# Adding a blog

You have created your first pages and now you want more, you want to create a blog!  
What differentiates normal pages from a blog :
- Blog pages have a special layout created by your theme.
- Blogs offer RSS feeds that your readers can subscribe to.
- You can add a comment section to your blog posts.

To create a blog, you must create a folder with the name displayed in the url of your blog. Then add this blog to your configuration.

**Example : Creating the CESTOLIV's blog**
The blog will have to be accessible at the address `https://cestoliv.com/blog` : you have to create a `blog` folder in the `source` folder : it is in this folder that you will find the posts.

You must then add the blog to the configuration :

```yaml
server:
    # server configuration

content:
    # content configuration

    blogs: [
        {
            dir: "./source/blog",
            title: "CESTOLIV's blog",
            description : "Un blog tech",
            category: "Technology",
            language: "fr",
            main_author: "cestoliv",
            authors: {
                "cestoliv": "me@cestoliv.com"
            }
        }
    ]
```

- **dir**: The folder where the blog content is located
- **title**: The blog title
- **description**: The blog description
- **category**: The blog category
- **language**: Blog language on 2 characters