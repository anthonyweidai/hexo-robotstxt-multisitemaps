# hexo-robotstxt-multisitemaps
Fork from leecrossley / hexo-generator-robotstxt

A very simple plugin to generate a robots.txt file automatically for [Hexo 3](https://npmjs.org/package/hexo).

## Usage

### Install

```
npm install hexo-robotstxt-multisitemaps --save
```

### Enable

Add `hexo-robotstxt-multisitemaps` to `plugins` in `_config.yml`.

``` yaml
plugins:
- hexo-robotstxt-multisitemaps
```

Add config for `robots.txt` to `_config.yml`.
``` yaml
robotstxt:
  useragent: "*"
  disallow:
    - /one_file_to_disallow.html
    - /2nd_file_to_disallow.html
    - /3rd_file_to_disallow.html
  allow:
    - /one_file_to_allow.html
    - /2nd_file_to_allow.html
    - /3rd_file_to_allow.html
  sitemap: 
    - /sitemap.xml
    - /baidu_sitemap.xml
```

### Settings & their defaults values

| Setting   | Description                                   | Default |
| --------- | --------------------------------------------- | ------- |
| useragent | Set the User-Agent                            | *       |
| disallow  | Disallow files or folders for this User-Agent |         |
| allow     | Allow files or folders for this User-Agent    |         |
| sitemap   | Set the path to your sitemap                  |         |

## Example
[How to auto generate sitemap and robots.txt for your web page powered by hexo](https://anthonydave.top/HTML/how-to-auto-generate-sitemap-and-robots-for-your-web-page-powered-by-hexo/)
## License

[MIT License](http://ilee.mit-license.org)
