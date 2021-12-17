```js
  ___ ____    _      ____                             _____                
 |_ _/ ___|  / \    / ___|  ___  ___ _   _ _ __ ___  |__  /___  _ __   ___ 
  | |\___ \ / _ \   \___ \ / _ \/ __| | | | '__/ _ \   / // _ \| '_ \ / _ \
  | | ___) / ___ \ _ ___) |  __/ (__| |_| | | |  __/_ / /| (_) | | | |  __/
 |___|____/_/   \_(_)____/ \___|\___|\__,_|_|  \___(_)____\___/|_| |_|\___|
 
```
Documentation
The implementation of this API and the client side app can be found on git hub
Quasar Fr
# Secure Zone



To serve these docs as a website:


```shell
npm i docsify-cli -g
docsify init
```
[Docsify Docs](https://docsify.js.org/#/quickstart)


This project uses the following technologies, Where the technologies are described further down this file, they are marked like this

- [x] They important for the project to work
- [?] Any one of these can be used
- [ ] Are viable alternatives but decided against them

Here are a list of all the tech used with their official docs, added short docs for each module that is relative to the project further down with install instructions and basic examples.

## Technologies 

- HTML
  - [HTML 5](https://www.w3schools.com/html/)
  - [Web Components](webComponents.org)
- CSS
  - [Sass](https://sass-lang.com/)
  - [UNO CSS](https://github.com/antfu/unocss)A
  - [Windi CSS](https://github.com/windicss/windicss)
  - [Critters](https://github.com/GoogleChromeLabs/critters)
  - [Unplugin](https://github.com/antfu/unplugin-icons)
- [PHP 7.4](https://www.php.net/)
  - [Laravel](https://laravel.com/)
  - [Lighthouse](https://lighthouse-php.com/)
  - [Sanctum](https://laravel.com/8.x/sanctum)
  - [CORS](https://lighthouse-php.com/5/getting-started/configuration.html#cors)
- [JavaScript (ES 2016)](https://www.javascript.com/)
  - JavaScript Modules
  - [Vue.js 3](https://vuejs.org/)
    - Vue Templates
    - [Vue Router](https://router.vuejs.org/)
    - [Vue Apollo for GraphQL](https://apollo.vuejs.org/)
    - [Vuex for State Management](https://next.vuex.vuejs.org/) or
    - [Pinia For State Management](https://pinia.esm.dev/introduction.html)
  - [Quasar](https://quasar.dev/)
  - [Quasar form Builder](https://github.com/baggachipz/q-form-builder-demo)
  - [Vite](https://vitejs.dev/)
  - [Vite Plugin Markdown](https://github.com/antfu/vite-plugin-md)
  - [Vite Server Side Rendering](https://vitejs.dev/guide/ssr.html)
  - [TypeScript](https://www.typescriptlang.org/)
  - [@vueuse/head](https://github.com/vueuse/head)
- [Node.js](https://nodejs.org/)
  - [NVM (Node version manager)](https://github.com/mvm-sh/nvm)
  - [Vite](https://vitejs.dev/)
  - [Quasar CLi](https://quasar.dev/)
- Database
  - [MySQL](https://www.mysql.com/)
  - [Redis](https://redis.io/)
- API
  - [GraphQL API](https://graphql.org/)
- Package Managers
  - [NPM / PNPM](https://www.npmjs.com/) or
  - [Yarn](https://yarnpkg.com/)
  - [Composer](https://getcomposer.org/)
- [Apache](https://www.apache.org/)
- [CentOS 8](https://www.centos.org/)
  - [Samba](https://www.linuxtechi.com/install-configure-samba-centos-8/)
- Version Control
  - [Git](https://git-scm.com/)

For each component there are installation instructions, usage instructions with some examples and where to get more help if needed

The checkboxes next to each item is the ones chose to use in the end. I also mention some other packages that I did not implement yet or nessesarily will, but some packages I sort of stumbled upon as I was reaching this and they sounded like they had something secial to offer.

## 1. CentOS 8

First we need to setup the CentOS 8 Server. There are quite a few steps. The items that is not checked is optional

- [x] [1.1 CentOS Install](centOS/1.1-centOSInstall.md)
- [x] [1.2 Firewall](centOS/1.2-firewall.md)
- [ ] [1.3 Midnight Commander](centOS/1.3-midnightCommander.md)
- [ ] [1.4 Disable SE Linux](centOS/1.4-seLinux.md)
- [x] [1.5 Install Mysql](centOS/1.5-mysql.md)
- [x] [1.6 Install PHP](centOS/1.6-php.md)
- [x] [1.7 Install Composer](centOS/1.7-composer.md)
- [x] [1.8 A Install Node.js](centOS/1.8-nodejs.md)
- [ ] [1.8 B Instal Node.js with NVM](centOS/1.8-nvm.md)
- [ ] [1.9 Install Yarn](centOS/1.9-yarn.md)
- [x] [1.10 Apache](centOS/1.10-apache.md)
- [x] [1.11 Git Install](centOS/1.11-git.md)
- [ ] [1.12 Install Samba](centOS/1.12-samba.md)
- [ ] [1.13 Set Static IP](centOS/1.13-networkSetStatic.md)

## 2. Virtual Hosts

> Setting up the virtual hosts has a trick to it when it comes to setting up sub-domains

Secure Zone runs as an API and as a client from two different VHOSTS so lets setup the VHOSTS

- [x] [2.1 Create the Directory Structure](vhosts/2.1-structure.md)
- [x] [2.2 Grant Permissions](vhosts/2.2-permissions.md)
- [ ] [2.3 Create Demo Pages for the Virtual Hosts](vhosts/2.3-demoPages.md)
- [x] [2.4 Set Up Local Hosts File](vhosts/2.4-hostsFile.md)
- [x] [2.5 Create New Virtual Host Files](vhosts/2.5-createConfFiles.md)


## 3. API with Laravel

In this section you only have to install 3.1 to 3.4. I explored the rest of the options but in the end Passport won yhe race.

Here is detailed instructions for passport auth:
- [x] [3.0 Login with Passport](API/3.0-loginWithPassport.md)

> Auth system

- [x] [3.1 Install Laravel via Composer](API/3.1-installWithComp.md)
- [x] [3.2 GraphQL with Laravel and Lighthouse](API/3.2-graphql.md)
- [x] [3.1 Install Lighthouse on API](API/3.3-lighthouse.md)
- [x] [3.4 Passport Authentication](API/3.4-passportAuth.md)
- [ ] [3.5 Sanctum Authentication](API/3.5-sanctum.md)
- [ ] [3.6 Auth with Bearer Token](API/3.6-bearerAuth.md)
- [ ] [3.7 Google 2FA](API/3.7-2fa.md)
- [ ] [3.8 Laravel DB Setup](API/3.8-data.md)
- [ ] [3.9 GraphQL Tools](API/3.9-graphqlTools.md)
- [ ] [3.10 Youtube Tutorial](API/3.10-youtube.md)
- [ ] [3.11 Laravel Artisan GUI](API/3.11-artisanGui.md)
- [ ] [3.12 Laravel Sanctum / Vue Apollo Authentication](API/3.12-sanctumApollo.md)

> Old secure zone laravel changes to get the old.secureZone to work

- [ ] [3.7 2 FA Implementation](API/3.7-2fa.md)

## 4. SecureZone Client Website

What I wanted to use is Vite, whatever I used with Vite does not matter and does not make any real difference, you can literally create one page with Vue and the next with Svelte and the next with React and the next with Lit-Element because Vite supports them all.

So the first JS Lib to install is Vite, when you install Vite it asks you which other lib you will be using, in this case I actually decided to go with Vue.js because it's got a smaller learning curve for future developers and has a good community and thousands of plugins and good support, you can use lit-element anywhere in between as it uses native web-components so it will have no influence.

- [ ] [4.0 Vite Lit-Element](client/4.0-litElement.md)
- [x] [4.1 Install Vue 3 CLI](client/4.1-vue.md)
- [x] [4.2 Vite and Quasar](client/4.2-viteQuasar.md)
- [x] [4.3 Sass Variables](client/4.3-sassVars.md)
- [x] [4.4 Uno CSS](client/4.4-unoCss.md)
- [ ] [4.5 Vue Apollo](client/4.5-vueApollo.md)
- [x] [4.6 Vue Router](client/4.6-vueRouter.md)
- [ ] [4.7 Vue Auto Routes](client/4.7-vueAutoRoutes.md)
- [x] [4.8 Vue Guards - Restrict Access](client/4.8-vueGuards.md)
- [ ] [4.9 Vuex Data Store](client/4.9-vuexDataStore.md)
- [ ] [4.10 Vite Markdown Plugin](client/4.10-vitePluginMd.md)
- [ ] [4.11 VueUse Head](client/4.11-VueUseHead.md)
- [x] [4.12 Quasar Cli](client/4.12-quasarCli.md)
- [ ] [4.13 CSS Tips](client/4.13-cssTips.md)
- [ ] [4.14 Pinia](client/4.14-piniaStateAndStore.md)
- [ ] [4.15 Critters CSS](client/4.15-critters.md)
- [x] [4.16 Quasar dotenv](client/4.16-dotenv.md) 
- [ ] [4.17 Quasar form builder](client/4.17-quasarFormBuilder.md)
- [ ] [4.18 GraphQL Vanilla JS](client/4.18-NoFramworkGraphQL.md)
- [ ] [4.19 `$apollo` outside vue component?](client/4.19-apolloOutsideVue.md)

## 5. Some apps to learn all about GraphQL

- [x] [5.1 Local dev Server X11 Forwarding](tools/5.1-x11forwarding.md)
- [x] [5.2 Vue GraphQL Tools & Tutotials](tools/5.2-vueGraphQLResources.md)
- [ ] [5.3 Scalable GraphQL server + Tooling and testing](tools/5.3-graphqlServerAndTools.md)
- [ x [5.4 GraphQL Electron Windows PLayground](tools/5.4-grapthQLElectron.md)
- [ ] [5.5 GraphQL Learning](tools/5.5-learingGraphQL.md)
- [ ] [5.6 GraphQL Code Genrator](https://github.com/dotansimha/graphql-code-generator)
- [ ] [5.7 Apollo Client Dev Tools](tools/5.7-apolloDevTools.md)
- [ ] [5.8 Altair GraphQL Cross Platform Client](tools/5.8-altairGraphQL.md)
- [x] [5.9 Creating GraphQL Queries with Laravel](tools/5.9-creatingGQLueries.md)
- [ ] [5.10 GraphQL Links and Options](tools/5.10-GQLFrameworkLinks.md)
- [ ] [5.11 Simplest GraphQL IDE with only CDN inlcudes](tools/5.11-GraphQLIDECDN.md)
- [ ] [5.12 GraphQL Live Query](tools/5.12-graphQLiveQuery.md)
- [ ] [5.13 Go GraphQL](https://github.com/hasura/go-graphql-client)
- [ ] [5.14 GrapQL PHP with out Larvel](https://github.com/webonyx/graphql-php) 
- [ ] [5.15 Graphinatort Standalone PHP GraphQL Serevr](https://github.com/infinityloop-dev/graphpinator)

## 6. Documentation for some Tools used

- [x] [6.1 Quasar Command List](quasar/6.1-commandList.md)
- [x] [6.2 Quasar boot files](quasar/6.2-bootFiles.md)
- [x] [6.3 Quasar Prefetch Feature](quasar/6.3-quasarPrefetch.md)
- [x] [6.4 Handling Assets](quasar/6.4-quasarAssets.md); 
- [x] [6.5 API Proxying for Dev](quasar/6.5-apiProxy.md)
- [x] [6.6 .env Processing](quasar/6.6-envProcess.md)
- [x] [6.7 Deploying a SPA](quasar/6.7-deployingOrBuilding.md)
- [x] [6.8 Open dev to Public](quasar/6.8-devForPublic.md)
- [x] *6.9 Quasar Components*
- [ ] [6.9.1 QSkeleton](quasar/6.9.1-qSkeleton.md)
- [x] [6.9.2 QMarkdown](quasar/6.9.2-qMarkdown.md)
- [ ] [6.9.3 Testing](quasar/6.9.3-quasarTesting.md) 
- [ ] [6.10 Sass Vars in JS](quasar/6.10-SassInJs.md)
 

## 7. Some hacks & Time savers

- [ ] [7.1 Graphql Mysql Schema](hacks/7.1-graphqlMysqlSchema.md)
- [x] [7.2 CORS (Cross-origin resource sharing)](hacks/7.2-cors.md)
- [ ] [7.3 Quick and Easy Static site genertor (Docs)](hacks/7.3-staticSiteGenHugo.md)

## 7.4 More tools for creating documentation

- [7.4.1 VuePress](https://vuepress.vuejs.org/)
- [7.4.2 MkDocs](https://www.libhunt.com/r/mkdocs)
- [7.4.3 sphinx](https://www.sphinx-doc.org/en/master/)
- [7.4.4 DocFX](libhunt.com/r/docfx)
- [7.4.5 pdoc - for Python Projects](https://pdoc.dev/)
- [7.4.6 Bookstack - wiki content built with PHP & Laravel](https://www.bookstackapp.com/)
- [7.4.7 Pycco - Literate-style documentation](https://pycco-docs.github.io/pycco/)
- [7.4.8 Python Cheatsheet](https://www.pythoncheatsheet.org/)\
- [7.4.9 Wiki.js](https://js.wiki/)
- [7.4.10 WKHTMLToPDF - Convert HTML to PDF using Webkit](https://wkhtmltopdf.org/)
- [7.4.11 Snappy](https://github.com/barryvdh/laravel-snappy)
- [7.4.12 Docusaurus](https://www.libhunt.com/r/docusaurus)
- [7.4.13 docsify](https://docsify.js.org/#/)
- [7.4.14 web.dev - source code for web.dev (by GoogleChrome)](https://www.libhunt.com/r/web.dev)
- [buefy](https://www.libhunt.com/r/buefy)

## 8 Deploy App

- [8.1 Files to update](deploy/8.1-filesToUpdate.md)