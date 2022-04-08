<template>
    <main>
        <LearnAboutSection/>
        <UpgradeSkillSection/>
    </main>
</template>

<script>
import LearnAboutSection from './mainComponents/LearnAboutSection.vue';
import UpgradeSkillSection from './mainComponents/UpgradeSkillSection.vue';

export default {
    name: 'IndexMain',
    components: {
        LearnAboutSection,
        UpgradeSkillSection,
    }
};
</script>

<style lang="scss" scoped>
</style>