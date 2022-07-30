<script lang="ts">
  let profilePic = 'images/profile.JPG'
  import ProfileImage from "./components/ProfileImage.svelte";
  import Title from "./components/Title.svelte";
  import Links from "./components/Links.svelte";
</script>

<div class="container">
  <!-- svelte-ignore a11y-img-redundant-alt -->
  <ProfileImage src={profilePic}/>
  <Title title="Natthaphol Uthumphirat"/>
  <div class="links-container">
    <Links link="https://www.facebook.com" linkName="Facebook"/>
    <Links link="https://www.instagram.com" linkName="Instagram"/>
    <Links link="https://toey-portfolio.vercel.app" linkName="Portfolio"/>
    <Links link="https://www.linkedin.com/in/natthaphol-uthumphirat" linkName="LinkedIn"/>
  </div>
</div>

<style>
  .container{
    /* background-color: rgba(255,0,0,0.2); */
    display: flex;
    flex-direction: column;
    width: 100vw;
    height: 100vh;
    max-width: 425px;
    max-height: 100vh;
    align-items: center;
    /* justify-content: center; */
  }

  .links-container{
    width: 100%;
    display: flex;
    flex-direction: column;
    gap: 12px;
  }
  
</style>