<template>
  <section class="student-work-container section">
    <StudentCard
      title="Fancy Time"
      imgSrc="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_800/v1613933809/Fancytime/Screenshot_2022-01-24_at_18-53-29_Vite_App_ijsmt9"
      altText="Fancy Time by Karis Ka"
      techStack="Vite, JavaScript"
      projectPage="Projects-FancyTime"
    /><StudentCard
      title="Scrappy Notes"
      imgSrc="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_800/v1613933809/scrappy notes/scrappy_shot_shurde"
      altText="Scrappy Notes By Daniel Briskman"
      techStack="VueJS"
      projectPage="Projects-Scrappy"
    /><StudentCard
      title="RPG Character Designer"
      imgSrc="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_800/v1613933809/RPG Character/rpg_screen_agdbvj"
      altText="RPG Character Designer Alston Chan"
      techStack="VueJS"
      projectPage="Projects-RPGC"
    />
    <StudentCard
      title="Escape Room"
      imgSrc="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_800/v1622764850/Escape%20Room/Screenshot_2021-06-03_escape-room_lt6ip6.png"
      altText="Escape Room Site Card"
      techStack="Vue, Firebase"
      projectPage="Projects-EscapeRoom"
    />
    <StudentCard
      title="Tech Times CMS"
      imgSrc="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_800/v1622764870/CMS/Tech_Times_CMS_nvokwg.png"
      altText="Tech Times CMS Card"
      techStack="Nuxt, TypeScript, MongoDB"
      projectPage="Projects-CMS"
    />
    <StudentCard
      title="Bone Apple Teeth"
      imgSrc="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_800/v1622764827/Richard/Screenshot_2021-05-31_Bone_Apple_Teeth_1_t7zgms.png"
      altText="Bone Apple Teeth Card"
      techStack="Nuxt, Firebase"
      projectPage="Projects-BoneAppleTeeth"
    />
    <StudentCard
      title="Japan"
      imgSrc="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_800/v1613933809/EthanJapan/Screenshot_2021-02-21_Visit_Japan_jr4nfj"
      altText="Japan by Ethan Liang"
      techStack="HTML, SCSS"
      projectPage="Projects-Japan"
    />
    <StudentCard
      title="Fantasy Kingdom"
      imgSrc="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_800/v1613933809/Fantasy Kingdom/Screenshot_2021-02-21_Galgudd_lorm1c"
      altText="Fantasy Kingdom by Charley Baluja and Daniel Briskman"
      techStack="HTML, SCSS"
      projectPage="Projects-FantasyKingdom"
    />
    <StudentCard
      title="Fire Emblem"
      imgSrc="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_800/v1613933809/Fire Emblem/attack_pdyrpw"
      altText="Fire Emblem By William Anderson"
      techStack="Node, MongoDB, Socket"
      projectPage="Projects-FireEmblem"
    />

    <StudentCard
      title="Loop"
      imgSrc="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_800/v1613933809/Loop/loop_dash_maxdej"
      altText="Loop by Class of 2020"
      techStack="Node, MongoDB"
      projectPage="Projects-Loop"
    />
    <StudentCard
      title="Jack Twenty-One"
      imgSrc="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_800/v1613933809/Jack21/Screenshot_2021-02-14_Jack_Twenty-One_pncx2g"
      altText="Jack 21 By Nick Melkadze"
      techStack="JavaScript, CSS"
      projectPage="Projects-Jack21"
    />
    <StudentCard
      title="Jang Foods"
      imgSrc="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_800/v1613933809/Jang Foods/Screenshot_2021-02-19_TechLife_Cafe_eavzef"
      altText="Jang Foods By Class of 2020"
      techStack="Node, MongoDB, Stripe"
      projectPage="Projects-Jang"
    />
    <StudentCard
      title="Pokemon Battle Sim"
      imgSrc="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_800/v1613933809/Pokemon/Screenshot_2020-05-25_PKMN_DUEL_nmiruw"
      altText="Pokemon By William Anderson"
      techStack="JavaScript, CSS"
      projectPage="Projects-Pkmn"
    />
    <StudentCard
      title="Tennis Reworked"
      imgSrc="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_800/v1613933809/Pong/pong1_bbnfeg"
      altText="Tennis Reworked By Brian Jiang"
      techStack="JavaScript, CSS"
      projectPage="Projects-Pong"
    />
    <StudentCard
      title="Cyberpunk Japan"
      imgSrc="https://res.cloudinary.com/dbopxlpuy/image/upload/c_scale,f_auto,w_800/v1613933809/CyberpunkJapan/yu2_n695bi"
      altText="Cyberpunk Japan By Kelly Yu"
      techStack="HTML, SCSS"
      projectPage="Projects-CyberJapan"
    />
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss">
.student-work-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, 26%);

  justify-content: space-around;

  width: 100%;
  margin: 4rem auto;
}
@include tablet {
  .student-work-container {
    grid-template-columns: repeat(auto-fit, 40%);
  }
}

@include phone {
  .student-work-container {
    grid-template-columns: repeat(auto-fit, 80%);
  }
}
</style>
