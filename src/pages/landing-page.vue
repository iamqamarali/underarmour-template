<template>
    <div class="landing-page">

        <top-banner></top-banner>
        <new-arrivals :arrivals="arrivals" ></new-arrivals>
        <collections-two-column :collections="twoColumnData"/>
        <collections-three-column :collections="threeColumnsData"/>
        <instagram-feed ></instagram-feed>

    </div>
</template>

<script>
import topBanner from '../components/landing-page/top-banner'
import newArrivals from '../components/global/new-arrivals'
import collectionsTwoColumn from '../components/global/collections-two-column'
import collectionsThreeColumn from '../components/landing-page/collections-three-column'
import instagramFeed from '../components/landing-page/instagram-feed'

export default {
    components:{
        topBanner : topBanner,
        newArrivals,
        collectionsTwoColumn ,
        collectionsThreeColumn,
        instagramFeed
    },
    data(){
        return {
            twoColumnData:[
                {
                    title :"Men's UA Breeze",
                    description : 'Wired different. Ready to take over.',
                    img : '/images/landing/section2/FW20_GLF_PlayoffPolo_Site_8_5_M.jpg',
                    link : '/category'
                },
                {
                    title :"Men's Polo Shirts",
                    description : 'Wired different. Ready to take over.',
                    img : '/images/landing/section2/FW20_Run_Breeze_Site_8_5_M.jpg',
                    link : '/category'
                },
            ],
            threeColumnsData:[
                {
                    title :"Women's Fly Fast Bottomss",
                    img : '/images/landing/three-column-banner/FW20_Run_FlyFast_Site_8_5.jpg',
                    link : '/listing'
                },
                {
                    title :"Women's Armour® Crossback Bras",
                    img : '/images/landing/three-column-banner/FW20_WMN_Seasonal_CrossbackMid_Site_8_5.jpg',
                    link : '/listing'
                },
                {
                    title :"Men's Polo Shirts",
                    img : '/images/landing/section2/FW20_Run_Breeze_Site_8_5_M.jpg',
                    link : '/listing'
                },
            ],
            arrivals:[
                {
                    link :'/men',
                    text : 'MEN'
                },
                {
                    link :'/men',
                    text : 'MEN'
                },
                {
                    link :'/men',
                    text : 'MEN'
                },
                {
                    link :'/men',
                    text : 'MEN'
                },
            ]
        }
    }
}
</script>
