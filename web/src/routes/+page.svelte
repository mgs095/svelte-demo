<script>
    import Hero from "../components/Hero.svelte";
    import HeroLeftRight from '../components/HeroLeftRight.svelte';
    import HeroImage from "$lib/assets/image-10.png";
    import HeroLeftRightImage from "$lib/assets/image-15.png";
</script>
<Hero 
    title="Productivity that flows with your life."
    content="Unleash your potential by harmonizing your daily tasks and habits with your unique energy rhythms."
    linkPath="/"
    linkTitle="Try for free"
    imageSrc={HeroImage}
/>

<HeroLeftRight 
    title="Features for finding focus"
    content="Harness our innovative feature set to propel your productivity power. Make every moment count, stress less."
    linkPath="/"
    linkTitle="Try for free"
    imageSrc={HeroLeftRightImage}
/>
