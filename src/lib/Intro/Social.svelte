<script>
  import data from "../../assets/social/social.json";
  import SocialButton from "./SocialButton.svelte";
</script>

<div class="social">
  <ul>
    {#each data as d}
      <SocialButton
        link={d.link}
        path={d.path}
        path2={d.path2 ? d.path2 : ""}
      />
    {/each}
  </ul>
</div>

<style>
  ul {
    list-style: none;
    padding: 0;
    margin: 0 auto;
    margin-bottom: 50px;
    display: flex;
    width: -webkit-fit-content;
    width: -moz-fit-content;
    width: fit-content;
  }
</style>
