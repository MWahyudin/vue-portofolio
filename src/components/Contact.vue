<template>
  <section id="contact">
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"
    />
    <div class="box">
      <div class="container">
      <div class="row">
          <div class="col-lg-12 text-center">
            <h2 class="section-heading text-uppercase">Contact</h2>
            <h3 class="section-subheading text-muted"></h3>
          </div>
        </div>
        <div class="row">
          <div class="col-lg-4 col-md-4 col-sm-4 col-xs-12"   v-for="obj in contacts" :key="obj.title">
            <div class="box-part text-center">
              <i :class="obj.icon" aria-hidden="true"></i>

              <div class="title">
                <h4>{{obj.title}}</h4>
              </div>

              <div class="text">
                <span>{{obj.text}}</span>
              </div>

              <a href="#">Learn More</a>
            </div>
          </div>

        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  data: () => ({
    contacts: [
      {
        icon: 'fa fa-instagram fa-3x',
        title: 'Instagram',
        text: '@Mwahyudin___',
      },
      {
        icon: 'fa fa-twitter fa-3x',
        title: 'twitter',
        text: '@Mwahyudin__',
      },
      {
        icon: 'fa fa-facebook fa-3x',
        title: 'Facebook',
        text: 'Fb.me/Mwahyu_Root',
      },
      {
        icon: 'fa fa-linkedin fa-3x',
        title: 'Linkedln',
        text: 'in/MWahyudin',
      },
    ],
  }),
};
</script>
