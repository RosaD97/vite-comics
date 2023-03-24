<script>
import Card from './Card.vue';

export default {
    components: {
        name: 'SeriesList',
        Card
    },
    data() {
        return {
            list: [
                {
                    "thumb": "https://static.dc.com/2023-03/LEGIONOB_Cv1_00111_DIGITAL.jpg?w=640",
                    "price": "$19.99",
                    "series": "DC'S LEGION OF BLOOM",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/FLS_Cv795_79511_DIGITAL.jpg?w=640",
                    "price": "$3.99",
                    "series": "THE FLASH",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/NTW_Cv102_10211_DIGITAL-1.jpg?w=640",
                    "price": "$16.99",
                    "series": "NIGHTWING",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/BMSMWF_Cv13_01311_DIGITAL.jpg?w=640",
                    "price": "$2.99",
                    "series": "BATMAN/SUPERMAN: WORLD'S FINEST",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/CTW_Cv53_05311_DIGITAL.jpg?w=640",
                    "price": "$3.99",
                    "series": "CATWOMAN",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/BA_Cv9_00911_DIGITAL.jpg?w=640",
                    "price": "$2.99",
                    "series": "BLACK ADAM",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/SM_LOST_Cv1_00111_DIGITAL.jpg?w=640",
                    "price": "$3.99",
                    "series": "SUPERMAN: LOST",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/SUPES_Cv2_00211_DIGITAL.jpg?w=640",
                    "price": "$4.99",
                    "series": "SUPERMAN",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/ROBIN_v3%20%28Cover%29.jpg?w=640",
                    "price": "$5.99",
                    "series": "ROBIN VOL. 3: SECRETS AND SHADOWS ",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/HQv3%20%28%20Cover%29.jpg?w=640",
                    "price": "$6.99",
                    "series": "HARLEY QUINN VOL. 3: VERDICT",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/MULTVTJ%20%28COVER%29.jpg?w=640",
                    "price": "$4.99",
                    "series": "MULTIVERSITY: TEEN JUSTICE",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.dc.com/2023-03/WW_Cv797_79711_DIGITAL.jpg?w=640",
                    "price": "$16.99",
                    "series": "WONDER WOMAN",
                    "type": "graphic novel"
                }
            ]
        }
    }
}
</script>

<template>
    <section>
        <h2 class="text">CURRENT SERIES</h2>
        <div>
            <div class="box">
                <Card :img="item.thumb" :title="item.series" v-for="item in list" class="card"></Card>
            </div>
        </div>
        <button class="text">LOAD MORE</button>
    </section>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/variables.scss' as *;


section {
    font-family: $font;
    color: $secondary-color;
    position: relative;
    margin-top: 20px;
}

.box {
    display: flex;
    flex-wrap: wrap;
    width: $Container;

    .card {
        flex-basis: calc(100% / 6);
        margin-bottom: 30px;

        :deep(img) {
            width: 90%;
            height: 150px;
            object-fit: cover;
            &:hover{
                cursor: pointer;
                filter: brightness(40%);
            }
        }
    }
}

h2 {
    position: absolute;
    top: -5.9375rem;
    left: 0;
    padding: 10px;
}

.text {
    background-color: $primary-color;
}

button {
    color: $secondary-color;
    border: none;
    font-family: $font;
    padding: 10px 40px 10px 40px;
    font-weight: 700;
    display: flex;
    margin: auto;
    &:hover{
        background-color: darken($primary-color, 20%);
        cursor: pointer;
    }
}</style>