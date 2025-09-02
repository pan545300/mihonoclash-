port: 3333
proxies:
  # 单个节点
proxy-providers:
  AP1:
    type: http
    url: https://oooooooooooooooosQ?clash=1&flag=meta  #修改你的机场1订阅地址
    interval: 86400
    health-check:
      enable: true
      url: https://www.gstatic.com/generate_204
      interval: 300
    override:
      additional-prefix: "[AP1]"
  AP2:
    type: http
    url: https://oooooooooooooooosQ?clash=1&flag=meta  #修改你的机场2订阅地址
    interval: 86400
    health-check:
      enable: true
      url: https://www.gstatic.com/generate_204
      interval: 300
    override:
      additional-prefix: "[AP2]"     

proxy-groups:
  - name: 🔃 自动选择
    type: url-test
    url: http://www.apple.com/library/test/success.html
    interval: 300
    tolerance: 100
    include-all: true

  - name: 🤖 ChatGPT
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇹🇼 台湾节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 🎥 YouTube
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇹🇼 台湾节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 🎥 Netflix
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇹🇼 台湾节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 🎥 Disney+
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 📲 Telegram
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇹🇼 台湾节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 📲 Twitter
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 📲 Instagram
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 📲 Facebook
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 🎵 Spotify
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 🔍 Google
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 🍎 Apple
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 💻 Microsoft
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 🎮Steam
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 🎮 Xbox
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 🎮 PlayStation
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 🎮 Nintendo
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 🎮 游戏
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 🔞 Porn
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 📲 TikTok
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 💸 Crypto
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 🎥 AppleTV
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 💳 PayPal
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 🌍 国外网站
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true

  - name: 🐟 漏网之鱼
    type: select
    proxies:
      - 🔃 自动选择
      - 🇺🇸 美国节点
      - 🇹🇼 台湾节点
      - 🇭🇰 香港节点
      - 🇯🇵 日本节点
      - 🇸🇬 新加坡节点
      - 🇰🇷 韩国节点
      - 🇬🇧 英国节点
      - 🌍 其他国家
      - DIRECT
    include-all: true


  - name: 🇺🇸 美国节点
    type: url-test
    url: http://www.apple.com/library/test/success.html
    interval: 300
    tolerance: 100
    filter: '^(?=.*((?i)🇺🇸|美国|波特兰|达拉斯|俄勒冈|凤凰城|费利蒙|硅谷|拉斯维加斯|洛杉矶|圣何塞|圣克拉拉|西雅图|芝加哥|(\b(US|United States)\b))).*$'
    include-all: true

  - name: 🇭🇰 香港节点
    type: url-test
    url: http://www.apple.com/library/test/success.html
    interval: 300
    tolerance: 100
    filter: '^(?=.*((?i)🇭🇰|香港|(\b(HK|Hong)\b))).*$'
    include-all: true

  - name: 🇯🇵 日本节点
    type: url-test
    url: http://www.apple.com/library/test/success.html
    interval: 300
    tolerance: 100
    filter: '^(?=.*((?i)🇯🇵|日本|川日|东京|大阪|泉日|埼玉|(\b(JP|Japan)\b))).*$'
    include-all: true

  - name: 🇹🇼 台湾节点
    type: url-test
    url: http://www.apple.com/library/test/success.html
    interval: 300
    tolerance: 100
    filter: '^(?=.*((?i)🇹🇼|TW|台湾)).*$'
    include-all: true

  - name: 🇸🇬 新加坡节点
    type: url-test
    url: http://www.apple.com/library/test/success.html
    interval: 300
    tolerance: 100
    filter: '^(?=.*((?i)🇸🇬|新加坡|狮|(\b(SG|Singapore)\b))).*$'
    include-all: true

  - name: 🇰🇷 韩国节点
    type: url-test
    url: http://www.apple.com/library/test/success.html
    interval: 300
    tolerance: 100
    filter: '^(?=.*((?i)🇰🇷|韩国|韓|首尔|(\b(KR|Korea)\b))).*$'
    include-all: true

  - name: 🇬🇧 英国节点
    type: url-test
    url: http://www.apple.com/library/test/success.html
    interval: 300
    tolerance: 100
    filter: '^(?=.*((?i)🇬🇧|英国|伦敦|(\b(UK|United Kingdom)\b))).*$'
    include-all: true

  - name: 🌍 其他国家
    type: url-test
    url: http://www.apple.com/library/test/success.html
    interval: 300
    tolerance: 100
    filter: '^(?!.*((?i)🇺🇸|美国|波特兰|达拉斯|俄勒冈|凤凰城|费利蒙|硅谷|拉斯维加斯|洛杉矶|圣何塞|圣克拉拉|西雅图|芝加哥|US|United States|🇭🇰|香港|HK|Hong|🇯🇵|日本|川日|东京|大阪|泉日|埼玉|JP|Japan|🇹🇼|TW|台湾|🇸🇬|新加坡|狮|SG|Singapore|🇰🇷|韩国|韓|首尔|KR|Korea|🇬🇧|英国|伦敦|UK|United Kingdom)).*$'
    include-all: true  

rules:
  # 国内网站
  - GEOSITE,cn,DIRECT
  # 🎥 Netflix
  - GEOSITE,netflix,🎥 Netflix
  # 🎥 Disney+
  - GEOSITE,disney,🎥 Disney+
  # 🎵 Spotify
  - GEOSITE,spotify,🎵 Spotify
  # 📲 Telegram
  - GEOSITE,telegram,📲 Telegram
  # 🎥 YouTube
  - GEOSITE,youtube,🎥 YouTube
  # 🔍 Google
  - GEOSITE,google,🔍 Google
  # 📲 Twitter
  - GEOSITE,twitter,📲 Twitter
  # 📲 Instagram
  - GEOSITE,instagram,📲 Instagram
  # 📲 Facebook
  - GEOSITE,facebook,📲 Facebook
  # 🍎 Apple
  - GEOSITE,apple@cn,DIRECT
  - GEOSITE,apple,🍎 Apple
  # 💻 Microsoft
  - GEOSITE,microsoft@cn,DIRECT
  - GEOSITE,microsoft,💻 Microsoft
  # 🎮Steam
  - GEOSITE,steam@cn,DIRECT
  - GEOSITE,steam,🎮Steam
  # 🎮 Xbox
  - GEOSITE,xbox,🎮 Xbox
  # 🎮 PlayStation
  - GEOSITE,playstation,🎮 PlayStation
  # 🎮 Nintendo
  - GEOSITE,nintendo@cn,DIRECT
  - GEOSITE,nintendo,🎮 Nintendo
  # 🎮 游戏
  - GEOSITE,category-games@cn,DIRECT
  - GEOSITE,category-games,🎮 游戏
  # 🤖 ChatGPT
  - GEOSITE,openai,🤖 ChatGPT
  - GEOSITE,anthropic,🤖 ChatGPT
  - GEOSITE,xai,🤖 ChatGPT
  # 🔞 Porn
  - GEOSITE,category-porn,🔞 Porn
  # 📲 TikTok
  - GEOSITE,tiktok,📲 TikTok
  # 💸 Crypto
  - GEOSITE,category-cryptocurrency,💸 Crypto
  # 🎥 AppleTV
  - GEOSITE,apple-tvplus,🎥 AppleTV
  # 💳 PayPal
  - GEOSITE,paypal,💳 PayPal
  # 🌍 国外网站
  - GEOSITE,geolocation-!cn,🌍 国外网站
  # GEOIP规则
  - GEOIP,private,DIRECT,no-resolve
  - GEOIP,google,🔍 Google
  - GEOIP,telegram,📲 Telegram
  - GEOIP,netflix,🎥 Netflix
  - GEOIP,twitter,📲 Twitter
  - GEOIP,CN,DIRECT
  # 🐟 漏网之鱼
  - MATCH,🐟 漏网之鱼
