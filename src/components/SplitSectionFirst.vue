<template>
  <section id="split-section" class="mb-2 d-flex w-100">
    <div id="image" class="w-50 d-flex justify-content-center align-items-center">
      <img src="../assets/img/h1-img-7n.png" alt="pizza-specials">
    </div>
    <div id="content" class="w-50 p-5">
      <ul class="text-start p-5">
        <li id="title">
          <ul>
            <li><h1 class="h2 fw-bold">SPECIALS*</h1></li>
            <li><p class="fs-small text-grey">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p></li>
          </ul>
        </li>
        <li>
          <div class="row">
            <div class="col-2">
              <h3 class="fw-bold text-brown">$10</h3>
            </div>
            <div class="col-10">
              <h3 class="fw-bold">COMBO PICCOLO</h3>
              <p class="fs-small text-grey">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Atque distinctio molestias, enim quod a maiores iusto, quidem sit sunt impedit nam laborum ratione ut sequi? Assumenda optio expedita inventore esse.</p>
            </div>
          </div>
        </li>
        <li>
          <div class="row">
            <div class="col-2">
              <h3 class="fw-bold text-brown">$20</h3>
            </div>
            <div class="col-10">
              <h3 class="fw-bold">COMBO MEZZO</h3>
              <p class="fs-small text-grey">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Corporis laborum velit incidunt illum ea, vel eveniet magni quisquam molestias sint quibusdam laboriosam!</p>
            </div>
          </div>
        </li>
        <li>
          <div class="row">
            <div class="col-2">
              <h3 class="fw-bold text-brown">$30</h3>
            </div>
            <div class="col-10">
              <h3 class="fw-bold">COMBO GRANDE</h3>
              <p class="fs-small text-grey">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Repellat porro perspiciatis sit voluptas praesentium, officiis eos officia ex.</p>
            </div>
          </div>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: 'SplitSectionFirst',
}
</script>

<style scoped>
#split-section {
  min-height: 600px;
}

#image{
  background-image: url('../assets/img/h1-img-4.jpg');
  background-size: cover;
  background-repeat: no-repeat;
}

.fs-small{
  font-size: 12px;
}

.text-grey{
  color: #b2b2b2;
}

.text-brown{
  color: #ab4027;
}
</style>