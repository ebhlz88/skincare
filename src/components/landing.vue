<template>
  <div>
    <img class="landimg" src="../assets/landing/landing.jpg" alt="landing" />
    <div id="landing">
      <div class="flex-column toleft">
        <p class="colorwhite applyheading">ARE YOU A CONSULTANT OR CLINIC?</p>
        <button class="applybtn colorblue">APPLY NOW</button>
      </div>
      <div class="flex-column center landdiv">
        <div>
          <div class="flex-row center">
            <h3 class="skinnotes">SKIN NOTES</h3>
            <img class="grouppng" src="../assets/landing/Group.png" alt="" />
          </div>
          <button class="landbutton">START YOUR SKIN JOURNEY</button>
        </div>
      </div>
    </div>
    <div id="features" class="flex-column colorwhite">
      <p class="heading2">FEATUrES</p>
      <div class="flex-row spacebtw">
        <div v-for="items in 3" :key="items" class="flex-column">
          <p class="heading3">DROP SHIP OUR PRODUCT</p>
          <p class="featuretxt">
            Use our backend to take bookings and manage your clients
          </p>
          <img class="grouppng" src="../assets/landing/Groupwhite.png" alt="" />
        </div>
      </div>
    </div>

    <div id="about" class="flex-column">
      <p class="heading2 colorblue">About the company</p>
      <div class="flex-row">
        <img class="docimg" src="../assets/landing/docpic.png" alt="doctor" />
        <div class="flex-column">
          <p class="docname">Dr. Divya v</p>
          <p class="docdesc">
            Divya Veluvolu has a wealth of experience in the cosmetic and
            skincare industry. She is one of the leading practitioners in her
            field.
          </p>
        </div>
      </div>
      <div class="flex-row docposition">
        <div v-for="items in 3" :key="items" class="flex-column jj">
          <div class="flex-row">
            <img
              class="docimgceo"
              src="../assets/landing/docpic.png"
              alt="doctor"
            />
            <div class="flex-column">
              <p class="docname">Dr. Divya v</p>
              <p class="colorblue">CEO</p>
            </div>
          </div>
        </div>
      </div>

      <div class="flex-column faq">
        <p class="heading2">faq</p>
        <p class="heading3 colorblue">how much do you charge?</p>
        <p class="docdesc">
          Skin notes is available for free, we only take a small commission fee
          from product sales and bookings (20%)
        </p>
      </div>
      <div class="flex-column faq toleft">
        <p class="heading3 colorblue">how much do you charge?</p>
        <p class="docdesc">
          Skin notes is available for free, we only take a small commission fee
          from product sales and bookings (20%)
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
/* top */
#landing {
  padding: 37px 39px;
  height: 650px;
}
.landimg {
  position: absolute;
  top: 0;
  height: 650px;
  width: 100%;
  z-index: -1;
}
.applyheading {
  font-size: 17px;
  font-weight: 700;
  margin-bottom: 0;
}
.landbutton {
  background-color: #334acb;
  color: white;
  padding: 14px 63px;
  font-size: 21px;
  font-weight: 700;
  margin-top: 18px;
}
.skinnotes {
  font-size: 36px;
  color: #071455;
}
.applybtn {
  background-color: rgba(255, 255, 255, 0.7);
  padding: 10px 103px;
  font-size: 15px;
  font-weight: 700;
  margin-top: 16px;
}
.grouppng {
  height: 37px;
  margin-left: 23px;
  width: 32px;
}
#features .grouppng {
  margin-left: 0;
}
.landdiv {
  height: 63%;
}

/* features */
#features {
  height: 373px;
  background-color: #334acb;
  align-items: center;
  padding-top: 41px;
}
.featuretxt {
  width: 154px;
  font-size: 11px;
  text-align: center;
}
#features .flex-row .flex-column {
  margin: 24px 43px;
  align-items: center;
}

/* About */
#about {
  align-items: center;
  padding: 41px 0;
}
#about .heading2 {
  margin-bottom: 43px;
}
.docimg {
  border-radius: 44px;
  height: 120px;
  margin: 0 38px;
}
.docname {
  color: #071455;
  font-weight: 600;
  text-transform: uppercase;
}
.docdesc {
  color: #334acb;
  font-weight: 500;
  width: 585px;
  font-size: 11px !important;
  text-transform: uppercase;
  text-shadow: 0.2px 0.2px #334acb;
}
.docimgceo {
  border-radius: 44px;
  height: 47px;
  margin: 0 20px;
}
.docposition {
  margin-top: 41px;
}
#about .docposition .jj {
  margin: 0px 60px;
}
#about .docposition .jj .docname,
.docdesc {
  margin: 0 0;
}
.docposition .docname,
.docdesc {
  font-size: 10px;
}
.faq {
  margin-top: 50px;
  width: 100%;
  padding: 28px 221px;
}
.faq .heading2 {
  font-size: 27px;
  font-weight: 800;
  text-transform: uppercase;
}
#about .heading3 {
  font-size: 15px;
}
.faq .docdesc {
  color: #071455;

  font-weight: 600;
  width: auto;
  font-size: 10px !important;
  text-transform: uppercase;
  text-shadow: none;
}
</style>
