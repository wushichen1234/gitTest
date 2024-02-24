项目：
1、个人博客
项目描述：项目为个人博客，记录平日生活点滴，项目分为前台界面和后台管理系统。
          前台界面包括对已发布的博文的展示以及一些自我介绍，网站介绍。
          后台管理系统包括对系统用户、权限、博文、评论的管理。
技术栈：vue2 + vue-cli + vue-router + vuex + Element-Ui组件库 + axios + less + webpack
项目负责：
           前台界面：
          （1）使用了vue-router进行路由配置，实现了前台界面的路由设计，定义路由路径和组件，通过一级和二级路由的划分，实现了页面
              的层级管理，提高了页面的组织和可维护性。
          （2）实现了生活感悟、情感日记、技术类、美好记忆的文章的分类和详情，点击详情后可访问博文具体内容，以及对热门文章、最新文章和随机文章的筛选。
          （3）实现了对已发布的博文数量、对发布博文的浏览量、对博文评价的总数量的统计。
          （4）实现了可通过搜索框输入关键字对博文的查询，并访问博文具体内容。
           后台系统：
          （1）使用了vue-router进行路由配置，实现了后台管理系统的路由设计，定义路由路径和组件，通过一级和二级路由的划分，实现了对页面的权限控制
               和登录验证，提供了良好的页面和交互体验。
          （2）实现了对管理系统用户用户名、密码和角色的管理，并可为对应的角色分配相应的权限。
          （3）实现了对博文信息和内容的管理，可对所有博文信息的标题、前言、类型统一管理，并使用开关（el-switch）管理该博文是否为热门文章。
               可根据博客标题来判断博客图片和博客内容是添加还是修改，通过输入博客标题后如果显示博客图片或博客内容的话，直接点击图片上传最新图片修改
               或者直接在富文本编辑器（mavon-editor）内修改，如果没显示则需在博文信息完善后添加博客图片和博客内容。
          （4）可对前台发布的一些不实评论予以删除。
           前台界面使用Webpack打包前使用路由懒加载异步组件，通过动态import语法的懒加载功能，将路由组件按需加载，提高页面的响应速度。
           将项目进行打包，将项目编译成HTML、CSS和JS文件，方便部署到服务器上,修改配置文件的publicPath,确保静态资源能正确加载,修改路由模式hash,适应服务器上部署的路径问题,确保路由能正确跳转和访问。
2、uni二手交易小程序
项目描述: 项目为一个基于uniapp开发的微信小程序,旨在提供一个方便大家出售二手商品的平台，项目包括首页、发闲置页、消息页和个人信息用户页面等功能。
技术栈：vue3 + vite + uniapp + node + axios + pinia + less
项目负责：
          （1）对axios进行了二次封装，添加请求拦截器和响应拦截器，对请求进行统一处理，提高代码的复用性和开发效率。使用Promise进行异步处理，更好地处理请求的成功和失败情况。
          （2）使用Pinia构建仓库，使用pinia-plugin-persistedstate插件实现数据持久化，实现了用户仓库的构建和持久化，在登录成功后，将返回的token存储到Pinia中的用户仓库，提升用户的体验和交互效果。
          （3）首页可访问好物列表，在好物列表未完全加载时会有骨架屏（skeleton）效果，目的是给用户一种页面正在加载的感觉，它只是使用占位符和动画效果来展示页面的大致布局和结构，待页面真实内容加载后会消失。
               在加载好物列表的时候采用分页加载，这样可以在需要时加载当前页面所显示的数据，可以避免一次性加载大量的数据，导致页面响应变慢。
          （4）可以点击发闲置来发布自己想要出手的商品，可以对商品进行描述和展示图片，发布后的商品会显示在好物列表中。
          （5）在浏览某一商品后买家如有意向，可先与卖家进行沟通交流，使用WebSocket双向通信功能，允许服务器和客户端之间双向发送和接收消息，实现实时的双向通信。沟通无问题后买家可以支付下单（模拟）购买该二手商品。
               在消息页可以同时作为买家和卖家进行沟通交流。
          （6）在个人页显示我发布的、我卖出的、我买到的二手商品的交易记录和统计。同时可对自己发布的二手商品进行下架管理。
3. cmcc装维app和cmcc装维管理系统
项目描述：该项目是一个基于vue3的供移动公司装维（宽带和专线）管理的app和系统，其中装维app用于为一线装维师傅接单处理工单的app，而装维管理系统用于为后台综调管理人员（平台审核人员）审核管理工单的平台。
技术栈：vue3 + vite + vantUI组件库（app） + element-plus组件库（系统） + vue-router + pinia + axios + less + Echarts可视化库 + webpack
项目负责：
          cmcc装维app：
          （1）使用插件amfe-flexible和postcss-pxtorem实现页面的响应式改变，通过修改html根节点的font-size大小来控制当前页面的rem样式，从而实现页面的适应性和响应式布局，提升了用户体验和页面的可访问性。
          （2）采用了Flex布局实现页面的划分和布局，提供了更灵活和强大的布局方式，使页面的结构和排版更加简洁、直观和易于维护，内容更易于阅读和理解，提升了页面的响应性和用户体验。
          （3）对axios进行了二次封装，添加请求拦截器和响应拦截器，对请求进行统一处理，提高代码的复用性和开发效率。
          （4）使用Pinia构建仓库，使用pinia-plugin-persistedstate插件实现数据持久化，实现了用户仓库的构建和持久化，在登录成功后，将返回的token存储到Pinia中的用户仓库，提升用户的体验和交互效果。
          （5）一线装维人员可以点击故障工单后查看待受理的故障工单，受理工单时需选择是否上门处理，受理成功也可回退受理，
               受理过程中若需上门处理还需上传上门图片和打卡上门签到地址（高德地图API AMapLoader），受理完成后系统会流转为自动归档，同时可以查看回单结果。
          （6）一线装维人员可以点击投诉工单后查看待受理的投诉工单，受理的工单都为上门类工单（所以无需选择是否上门，只需受理即可），受理成功也可回退受理，
               受理过程中上门处理还需上传上门图片和打卡上门签到地址（高德地图API AMapLoader），受理完成后需等待一级和二级综调质检（平台审核），质检完后归档，并可查看回单结果。


          
