<script lang="ts">
  let profilePic = 'images/profile.JPG'
  import ProfileImage from "./components/ProfileImage.svelte";
  import Title from "./components/Title.svelte";
  import Links from "./components/Links.svelte";
</script>

<div class="container">
  <!-- svelte-ignore a11y-img-redundant-alt -->
  <div class="centerdiv top"><ProfileImage src={profilePic}/></div>
  <div class="centerdiv bottom"><Title title="Natthaphol Uthumphirat"/>
    <div class="links-container">
      <Links link="https://www.facebook.com" linkName="Facebook"/>
      <Links link="https://www.instagram.com" linkName="Instagram"/>
      <Links link="https://toey-portfolio.vercel.app" linkName="Portfolio"/>
      <Links link="https://www.linkedin.com/in/natthaphol-uthumphirat" linkName="LinkedIn"/>
    </div></div>
</div>

<style>
  .container{
    /* background-color: rgba(255,0,0,0.2); */
    display: flex;
    flex-direction: column;
    width: 100vw;
    height: 100vh;
    max-width: 425px;
    align-items: center;
    /* justify-content: center; */
  }

  .top{
    height: 50vh;
  }
  .bottom{
    height: 50vh;
  }

  .links-container{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 12px;
  }
  
</style>