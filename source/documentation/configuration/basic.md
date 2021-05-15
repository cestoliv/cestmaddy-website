# Basic Configuration

The configuration is done in the `config.yml` file and in the `.env` file. The minimal configuration is the following, let's unpack it!

## config.yml
```yaml
server:
    hide_html_extension: true
    domain: "https://cestmaddy.com"

content:
    title: "My website"
    language: fr
    header_file: "./source/header.md"
    footer_file: "./source/footer.md"
    theme: "clean"
```

### Server part
The first part, server, configures the server (logical)

- **hide_html_extension**: If set to True, the extensions `.html` will be hidden (`domain.com/hello.html` will become `domain.com/hello`)
- **domain**: The domain of your website (you can define a sub-folder), useful for sitemaps, RSS feeds, etc.

### Content part
Here is now the configuration of your content!

- **language**: The main language of your content, on two characters
- **header_file**: The local path to the markdown file that contains your header
- **footer_file**: The local path to the markdown file that contains your footer
- **theme**: The theme of your site: here is a list of available themes