<script lang="ts">
  let profilePic = 'images/profile.JPG'
  let facebookLogo = 'images/facebook.svg'
  let githubLogo = 'images/github.svg'
  let linkedInLogo = 'images/linkedin.svg'
  let wwwLogo = 'images/www.svg'

  import ProfileImage from "./components/ProfileImage.svelte";
  import Title from "./components/Title.svelte";
  import Links from "./components/Links.svelte";

  let title = `Natthaphol <br/>Uthumphirat`
</script>

<div class="container">
  <!-- svelte-ignore a11y-img-redundant-alt -->
  <div class="top">
    <ProfileImage src={profilePic}/>
    <Title {title} />
  </div>
  <div class="bottom">
    <div class="links-container">
      <Links logoSrc={facebookLogo} link="https://www.facebook.com/dekaiser02354" linkName="Facebook"/>
      <Links logoSrc={githubLogo} link="https://github.com/toey02354" linkName="Github"/>
      <Links logoSrc={wwwLogo} link="https://toey-portfolio.vercel.app" linkName="Portfolio"/>
      <Links logoSrc={linkedInLogo} link="https://www.linkedin.com/in/natthaphol-uthumphirat" linkName="LinkedIn"/>
    </div>
  </div>
</div>

<style>
  .container{
    /* background-color: rgba(255,0,0,0.2); */
    display: flex;
    flex-direction: column;
    width: 100vw;
    height: 100vh;
    align-items: center;
    /* justify-content: center; */
    overflow-x: hidden;
  }

  .top{
    height: 50vh;
    position: relative;
  }
  .bottom{
    height: 50vh;
    width: 90vw;
    min-width: 400px;
  }

  .links-container{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 12px;
    margin: 2rem auto;
  }
  
</style>