# vue-douban-movie
The doubanMovie project was overwrited by VUE
## Attention please
1. Because the doubanMovieAPI doesnot offer the admin for developer to reslove the CORS ,but that can be resolved when you are using Vue-cli.
you can find the proxyTable in the document of `index.js`.
2. Then you need to reset the content, just like this 
    proxyTable: {
      '/api':{
        target:'https://api.douban.com/v2',
        changeOrigin:true,//must set
        pathRewrite:{
          '^/api':''
        }
    }
3. Frankly , the step has been finished ,and you can use the API in your codes.
