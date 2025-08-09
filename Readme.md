clash verge 脚本

```javascript
/**
 * 人生不止色色
 * 不要让小头控制大头
 */
const NoSexRules = [
  "DOMAIN-SUFFIX,pixiv.net,REJECT",
  "DOMAIN-SUFFIX,wnacg.com,REJECT",  
  "DOMAIN-KEYWORD,porn,REJECT",
  "DOMAIN-KEYWORD,spank,REJECT",
  "DOMAIN-KEYWORD,xxx,REJECT",
  "DOMAIN-SUFFIX,18comic.vip,REJECT",
  "DOMAIN-SUFFIX,www.xnxx.com,REJECT",
  "DOMAIN-SUFFIX,xhamster.com,REJECT",
  "DOMAIN-SUFFIX,xvideos.com,REJECT",       
  "DOMAIN-SUFFIX,spankbang.com,REJECT",
  "DOMAIN-SUFFIX,chaturbate.com,REJECT",
  "DOMAIN-SUFFIX,livejasmin.com,REJECT",
  "DOMAIN-SUFFIX,onlyfans.com,REJECT",
];
function main(config) {
  let oldrules = config["rules"];
  config["rules"] = NoSexRules.concat(oldrules);
  return config;
}
```


