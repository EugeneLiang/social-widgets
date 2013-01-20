# Social widgets

Likes, shares and things like that.



## Table Of Contents

* [share](#share)
* [count-shares](#count-shares) (JSON with number of shares)



<a name='share'></a>
## share

<table>
  <tr>
    <th>Network</th>
    <th>URL</th>
    <th>Documentation</th>
  </tr>
  <tr>
    <td>Facebook</td>
    <td>https://facebook.com/sharer/sharer.php?u=http://google.com</td>
    <td></td>
  </tr>
  <tr>
    <td>Twitter</td>
    <td>http://twitter.com/share?url=http://google.com</td>
    <td></td>
  </tr>
  <tr>
    <td>Twitter</td>
    <td>https://twitter.com/intent/tweet?url=http://google.com</td>
    <td></td>
  </tr>
  <tr>
    <td>Google Plus</td>
    <td>https://plus.google.com/share?url=http://google.com</td>
    <td>[link](https://developers.google.com/+/plugins/share/#sharelink)</td>
  </tr>
  <tr>
    <td>Linked In</td>
    <td>http://www.linkedin.com/shareArticle?url=http://google.com</td>
    <td>[link](https://developer.linkedin.com/documents/share-linkedin)</td>
  </tr>
  <tr>
    <td>VK</td>
    <td>http://vkontakte.ru/share.php?url=http://google.com</td>
    <td>[link](http://vk.com/developers.php?oid=-17680044&p=Share)</td>
  </tr>
  <tr>
    <td>Odnoklassniki</td>
    <td>http://www.odnoklassniki.ru/dk?st.cmd=addShare&st.s=1&st._surl=http://google.com</td>
    <td></td>
  </tr>
</table>



<a name='count-shares'></a>
## count-shares

Returns JSON with a number of shares for a page.

```
{
    "facebook": 5461703,
    "twitter": 11876867,
    "vk": 2462,
    "odnoklassniki": 547,
    "linkedin": 18113
}
```


### API

Example: `/shares/php/main.php?url=http://www.google.com&networks=facebook,twitter`

#### url (required)

`www.domain.com` and `domain.com` are different websites for Twitter and Odnoklassniki.

#### networks

Comma separated. `facebook`, `twitter`, `linkedin`, `vk` or `odnoklassniki`.

Default: Facebook and Twitter.