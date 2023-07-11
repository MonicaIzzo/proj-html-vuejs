<script>
import GammerShop from './section/GammerShop.vue';
import LatestNews from './section/LatestNews.vue';
import LiveStraming from './section/LiveStraming.vue';
import OurExtremFeature from './section/OurExtremFeature.vue';
import TeamMembers from './section/TeamMembers.vue';
import Testimonials from './section/Testimonials.vue';
import TredingBattle from './section/TredingBattle.vue';
import TrendingGames from './section/TrendingGames.vue';
import UpComingMatch from './section/UpComingMatch.vue';
import YearExperince from './section/YearExperince.vue';

export default {
    components: { GammerShop, LatestNews, LiveStraming, OurExtremFeature, TeamMembers, Testimonials, TredingBattle, TrendingGames, UpComingMatch, YearExperince },
};


</script>

<template>
    <section id="main">
        <YearExperince />
        <OurExtremFeature />
        <LiveStraming />
        <TredingBattle />
        <TrendingGames />
        <UpComingMatch />
        <TeamMembers />
        <Testimonials />
        <GammerShop />
        <LatestNews />
    </section>
</template>

<style lang="scss" scoped>
#main {
    background-color: white;
}
</style>