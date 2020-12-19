<template>
<div class="p-5 arkaplan" id="anlasmalar">
<div class="container">
<img src="https://www.indiafilings.com/learn/wp-content/uploads/2018/08/Odisha-Partnership-Firm-Registration.jpg" class="resim" />
<div class="row row-cols-1 row-cols-md-4 g-3">
  <div class="col">
    <div class="card text-center h-100">
      <img src="https://cdn.sanity.io/images/9kdepi1d/production/65c832d202a503b15d99e628f4313782f3ef50db-300x62.png" class="card-img-top" alt="...">
      <div class="card-body">
        <h5 class="card-title">Kodluyoruz</h5>
        <p class="card-text">Topluluğumuz Kodluyoruz desteği ile kurulmuştur ve ilk günden beri sonsuz bir destek sunmaktalar. Onları çok seviyoruz! Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa adipisci et accusantium explicabo officia omnis consequuntur corrupti voluptatum, ducimus excepturi. Veritatis laboriosam aliquid sequi ad eligendi eius aspernatur expedita esse. Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
      </div>
    </div>
  </div>
  <div class="col">
    <div class="card text-center h-100">
      <img src="https://pbs.twimg.com/profile_images/1049218676342312966/cxfHMBfc_400x400.jpg" class="card-img-top center" style="width: 200px; height: 200px;">
      <div class="card-body">
        <h5 class="card-title">Elma Yayınevi</h5>
        <p class="card-text">Elma Yayınevi'nin web sitesi elmayayinevi.com'dan yapacağınız kitap alışverişi topluluk üyelerimize özel %35 indirimli! Ayrıca okuyancocuk.com'da kablosuzbeyin indirim kodunu kullanarak  Pötikare Yayıncılık, Sola Kidz, Sola Unitas, Elma Yayınevi ve Elma Çocuk markalarına ait kitaplarda ek %5 indirim!</p>
      </div>
    </div>
  </div>
  <div class="col">
    <div class="card text-center h-100">
      <img src="https://dodact.com/wp-content/uploads/2020/10/Varlik-1.png" class="card-img-top center" style="width: 200px; height: 200px;">
      <div class="card-body">
        <h5 class="card-title">Dodact</h5>
        <p class="card-text">Karşılıklı partnershiplik. Lorem ipsum dolor sit amet consectetur adipisicing elit. Exercitationem asperiores tempora possimus similique, dicta expedita nisi nam labore esse excepturi quas aut, voluptas aliquam odio itaque eos unde? Soluta, sunt!</p>
      </div>
    </div>
  </div>
  <div class="col">
    <div class="card h-100 text-center">
      <img src="https://www.vodafone.com.tr/KaraKartal/assets/img/yemeksepeti-960x280.jpg" class="card-img-top" alt="...">
      <div class="card-body">
        <h5 class="card-title">Yemeksepeti</h5>
        <p class="card-text">Hadi inşallah bir gün be!</p>
      </div>
    </div>
  </div>
</div>
</div>
</div>
</template>

<script>
import InfiniteSlideBar from 'vue-infinite-slide-bar'
export default {
  components: {
    InfiniteSlideBar,
  }
}
</script>

<style scoped>
.center {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 50%;
}
.arkaplan {
    position: relative;
    overflow: hidden;
    padding: 16px;
    /* height: 100%; */
}
.resim {
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    opacity: 0.6;
}
</style>