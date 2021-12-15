<template>
  <section>
    <div class="container" id="recent_articles">
           <div class="row justify-content-center">
            <!-- title  -->
            <div class="col-lg-7 px-0">
                <h5  id="title">
                     What The Crities Say
                </h5>
                <div id="subtitle">
                    TESTIMONIALS FROM AROUND THE WORLD
                </div>
            </div>
            <!-- Read  -->
            <div class="col-lg-2" id="btn_read">
                <button>
                    Read All Testimonials
                </button>
            </div>
        </div>

          <!-- Card and description  -->

          <div class="row justify-content-center"  id="card_description">
              <div class="col-lg-6" id="principal_card">
                <img class="img_recent_articles" src="../assets/20-Tips-600x353.jpg" alt="book">

                <div id="creativity_tips">
                  20 Creativity Tips
                </div>

                <span class="date">By admin | October 24th,2019 | Categories Event, Tips &amp; Tricks</span>
                
                <p>
                  Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Donec velit neque, auctor sit amet aliquam vel, ullamcorper sit amet
                </p>
              </div>

              <!-- other testimoniance  -->
              <div class="col-lg-3" id="secondary_card">
                  <div class="other_mini_card">
                      <img class="img_recent_articles" src="../assets/thumb-13-2x-320x202.jpg" alt="booklist">
                      <div>
                        What's On Your Booklist?
                      </div>
                      <span class="date">
                        October 24th 2019 | 0 comments
                      </span>
                  </div>
                  
                  <div class="other_mini_card">
                      <img class="img_recent_articles" src="../assets/thumb-08-2x-320x202.jpg" alt="travelguide">
                      <div>
                        Istambul Travel Guide
                      </div>
                      <span class="date">
                        October 24th 2019 | 0 comments
                      </span>
                  </div>
                
              </div>
          </div>
    </div>    
        
        
  </section>
</template>

<script>
export default {
  name: 'recentArticles',
  props: {

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section{
  background-color: #f3ece3;
}
#recent_articles{
    padding: 60px 0;
    position: relative;
    #card_description{
      margin-top: 30px;
    }
    #title{
        font-weight: bold;
        font-family: serif;
    }
    #subtitle{
        font-size: .7rem;
        color: #3da698;
    }
    #creativity_tips{
      margin-top: 20px;
    }      
    #btn_read{
        display: flex;
        align-items: center;
    }      
    button{
        color: white;
        font-weight: bold;
        padding: 7px 0;
        width: 100%;
        border-radius: 5px;
        background-color:#f3b329 ;
        border-style: none;
        font-size: .6rem;
    }
  .date{
      font-size: .6rem;
    }
  p{
    font-size: .9rem;
    margin-top: 10px;
  }
  // card 
  #principal_card{
    padding: 30px;
    background-color: white;
    margin-right: 30px;
  }
  #secondary_card{
    padding: 30px;
    background-color: white;
  }
  .img_recent_articles{
    width: 100%;
    margin-bottom: 10px;
  }
  .other_mini_card{
    margin-bottom: 30px;
  }
}
</style>