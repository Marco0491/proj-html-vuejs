<template>
    <main>
        <LearnAboutSection/>
        <UpgradeSkillSection/>
        <CoursesSection/>
        <TestimonialSection/>
        <BlogSection/>
        <NewsletterSection/>
    </main>
</template>

<script>
import LearnAboutSection from './mainComponents/LearnAboutSection.vue';
import UpgradeSkillSection from './mainComponents/UpgradeSkillSection.vue';
import CoursesSection from './mainComponents/CoursesSection.vue';
import TestimonialSection from './mainComponents/TestimonialSection.vue';
import BlogSection from './mainComponents/BlogSection.vue';
import NewsletterSection from './mainComponents/NewsletterSection.vue';

export default {
    name: 'IndexMain',
    components: {
        LearnAboutSection,
        UpgradeSkillSection,
        CoursesSection,
        TestimonialSection,
        BlogSection,
        NewsletterSection,
    }
};
</script>

<style lang="scss" scoped>
@import '../assets/styles/variables.scss';
</style>
