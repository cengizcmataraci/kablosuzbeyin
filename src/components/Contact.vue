<template>
  <div class="p-5 arkaplan" id="iletisim">
    <img
      src="https://lh3.googleusercontent.com/proxy/4o9iBgd1Z4Ce58eO9WpVeuI7ZLOVirPBAY1g-waobk-Q0SfdevCvli_PcoxpkQdwiKz7VoSbe5Zmtq5t4esVjRr_hwulxU89URHaOYmjXRHV7YXhEGoAqxsw4jQq4b_FfNHFXpHS8RsompBeNXcOjo5K5xxHNSiQLzBUOgBVUiGnKryDMcC21mUuamz2UjlZirAqBUJvz0XdWp2vKdgQLW1d_LF2wA"
      class="resim"
    />
    <h1 class="text-center">Bize Ulaşın</h1>
    <div class="card container border-danger mb-3 bg-transparent">
      <div class="card-body container">
        <div class="row g-2">
          <div class="col-md">
            <form class="form-floating">
              <input
                type="email"
                class="form-control"
                id="floatingInputValue"
                placeholder="name@example.com"
                value="test@example.com"
              />
              <label for="floatingInputValue">Mail Adresiniz</label>
              <div class="form-floating mt-3">
                <textarea
                  class="form-control"
                  placeholder="Leave a comment here"
                  id="floatingTextarea2"
                  style="height: 100px"
                ></textarea>
                <label for="floatingTextarea2">Mesajınız</label>
              </div>
              <div class="mt-3">
                <button class="btn btn-primary">Gönder</button>
              </div>
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.arkaplan {
    position: relative;
    overflow: hidden;
    padding: 16px;
}
.resim {
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: auto;
    opacity: 0.6;
}
</style>
