<template>
    <section>
        <div class="container">
            <div class="row justify-content-between">
                <div class="col-lg-6" id="jumbotron">
                    <h2>
                        Damon Vaughn
                    </h2>
                    <p>
                        Best-selling author and the most influential public intellectual in the western world right now.
                    </p>
                    <cite>
                        - The New York Times
                    </cite>
                    <div id="prev_next">
                        <i class="fas fa-arrow-left arrow"></i> <i class="fas fa-arrow-right arrow"></i>
                    </div>
                </div>
            </div>
         
        </div>
        <div id="latest_book">
            <div id="image_latest_book">
                <img src="../assets/book-widget.png" alt="latest_book">
            </div>
            <div id="description_latest_book">
                <h3>
                    Latest Book Release
                </h3>
                <h4>
                    D. VAUGHN AUTOBIOGRAPHY
                </h4>
                <p>
                    Vestubulum tristique turpis in ipsum egestas lobortis. Duis maximus bibendum volupat. Lorem ipsum dolor sit amet.
                </p>
            </div>
            <div id="buy_on">
                <button class="btn_latest_book" id="btn_amazon">
                    <i class="fab fa-amazon"></i> Buy On Amazon
                </button>
                <button class="btn_latest_book" id="btn_appstore">
                   <i class="fab fa-apple"></i> Buy On AppStore
                </button>
            </div>
        </div>
       
    </section>
   
    
</template>

<script>
export default {
  name: 'msJumbrotron',
  props: {
    
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Shalimar&display=swap');
section{
    position: relative;
}
#jumbotron{
    color: white;
    h2{
        font-family: Shalimar;
        color: #f3b329;
        font-weight: bold;
        font-size: 50px;
    }
    p{
        font-weight: bold;
        font-size: 1.8rem;
    }
    cite{
        color: #bec6be;
    }
    #prev_next{
        margin: 20px 0;
        .arrow{
            padding: 15px;
            font-size: 0.7rem;
            background-color: rgba(0, 0, 0, 0.849);
            cursor: pointer;
        }
    }
}
#latest_book{
    background-color: white;
    position: absolute;
    bottom: 0;
    right: 0;
    display: flex;
    flex-wrap: wrap;
    width: 35%;
    padding: 30px;
    #image_latest_book{
        width: 40%;
    }
    img{
        max-width: 100%;
        height: auto;
    }
    h3{
        font-size: 15px;
        font-weight: bold;
    }
    h4{
        font-size: 14px;
        color: #f3b329 ;
    }
    p{
        font-size: 12px;
    }
    #description_latest_book{
        width: 60%;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
    #buy_on{
        width: 100%;
        .btn_latest_book{
            width: 50%;
            border-style: none;
            padding: 7px 0;
            font-size: .7rem;
        }
        #btn_amazon{
            border: 1px solid black;
            border-top-left-radius: 5px;
            border-bottom-left-radius: 5px;
        }
        #btn_appstore{
            border: 1px solid black;
            border-left: none;
            border-top-right-radius: 5px;
            border-bottom-right-radius: 5px;
        }
    }
}
</style>