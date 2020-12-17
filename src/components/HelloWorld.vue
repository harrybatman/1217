<template lang="pug">
.newsContainer
  .newsFlex
    .newsItem(v-for= "item in news")
      .newsImg(:style="{'background-image': 'url(' + item.img + ')'}")
      .newsTitle {{item.title}}
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },
  data(){
    return{
      news:[
        {img:'https://scontent-hkt1-1.xx.fbcdn.net/v/t1.0-9/131432557_2857342427878078_5101152320245473747_o.jpg?_nc_cat=106&ccb=2&_nc_sid=730e14&_nc_ohc=zJlcTdj4Er8AX8yNSny&_nc_ht=scontent-hkt1-1.xx&oh=6bf7ed680bfcd6f5b4f0774b67865b9b&oe=6001890E', title:'hey'},
        {img:'https://scontent-hkt1-1.xx.fbcdn.net/v/t1.0-9/131589570_2857342401211414_7356372572954515507_o.jpg?_nc_cat=100&ccb=2&_nc_sid=730e14&_nc_ohc=RXfWojNFdqQAX8wLQee&_nc_ht=scontent-hkt1-1.xx&oh=9dc5dab84b0a8400a11a58997554841a&oe=60001846', title:'hi'},
        {img:'https://scontent-hkt1-1.xx.fbcdn.net/v/t1.0-9/131226962_2857342394544748_8902686430400113345_o.jpg?_nc_cat=100&ccb=2&_nc_sid=730e14&_nc_ohc=oFfNO1VX5ugAX-mbZvc&_nc_ht=scontent-hkt1-1.xx&oh=cb12d7b85ff42dd0b9384239b56982b5&oe=5FFF159E', title:'fuck u'},
      ],
    };
  },
};

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass">
.newsFlex
  display: flex
  flex-direction: row
  //border: 1px solid
  width: 1000px
  margin: auto
  justify-content: space-between
.newsItem
  //border: 1px solid red
  //width: 200px
  //height: 200px
.newsImg
  //border: 2px solid green
  width: 200px
  height: 200px
  background-size: cover
  display: flex
  flex-direction: column
  justify-content: pace-between
  margin-bottom: 25px
  border-radious: 24
.newsTitle

</style>
