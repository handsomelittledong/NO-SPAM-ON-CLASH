# clash verge 脚本

下定决心戒色时写的

为了屏蔽色情内容但是不想下梯子

所以写了一个脚本

希望大家可以脱离低级趣味

远离色情

过上更加健康快乐的生活


```javascript
/**
 * 人生不止色色
 * 不要让小头控制大头
 */
const NoSexRules = [
  "DOMAIN-SUFFIX,pixiv.net,REJECT",//扪心自问一下，你上p站到底是为了看色图还是为了看全年龄作品
  "DOMAIN-SUFFIX,wnacg.com,REJECT",  
  "DOMAIN-KEYWORD,porn,REJECT",
  "DOMAIN-KEYWORD,spank,REJECT",
  "DOMAIN-KEYWORD,xxx,REJECT",
  "DOMAIN-KEYWORD,sex,REJECT",
  "DOMAIN-KEYWORD,r18,REJECT",
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



