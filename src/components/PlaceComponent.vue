<template>
    <div class="bg-red-500" v-for="(item, index) in items" :key="index">
        <img :src="item.coverimage" alt="">
        <h3>{{ item.id }}.{{ item.name }}</h3>
        <p>{{ item.detail }}</p>
    </div>
</template>

<script>

export default {
    name: 'Place',
    props: ["addPlace"],
    data() {
        return {
            items: [
                {
                    id: 1,
                    name: "Phi Phi Islands",
                    detail: "Phi Phi Islands are a group of islands in Thailand between the large island of Phuket and the Malacca Coastal Strait of Thailand.",
                    coverimage: "https://www.melivecode.com/attractions/1.jpg"
                },
                {
                    id: 2,
                    name: "Eiffel Tower",
                    detail: "Eiffel Tower is one of the most famous structures in the world. Eiffel Tower is named after a leading French architect and engineer. It was built as a symbol of the World Fair in 1889.",
                    coverimage: "https://www.melivecode.com/attractions/2.jpg"
                },
                {
                    id: 3,
                    name: "Times Square",
                    detail: "Times Square has become a global landmark and has become a symbol of New York City. This is a result of Times Square being a modern, futuristic venue, with huge advertising screens dotting its surroundings.",
                    coverimage: "https://www.melivecode.com/attractions/3.jpg"
                },
                {
                    id: 4,
                    name: "Mount Fuji",
                    detail: "Mount Fuji is the highest mountain in Japan, about 3,776 meters (12,388 feet) situated to the west of Tokyo. Mount Fuji can be seen from Tokyo on clear days.",
                    coverimage: "https://www.melivecode.com/attractions/4.jpg"
                },
                {
                    id: 5,
                    name: "Big Ben",
                    detail: "Westminster Palace Clock Tower which is most often referred to as Big Ben. This is actually the nickname for the largest bell that hangs in the vent above the clock face.",
                    coverimage: "https://www.melivecode.com/attractions/5.jpg"
                },
                {
                    id: 6,
                    name: "Taj Mahal",
                    detail: "The Taj Mahal or Tachomhal is a burial building made of ivory white marble. The Taj Mahal began to be built in 1632 and was completed in 1643.",
                    coverimage: "https://www.melivecode.com/attractions/6.jpg"
                },
                {
                    id: 7,
                    name: "Stonehenge",
                    detail: "Stonehenge is a monument prehistoric In the middle of a vast plain in the southern part of the British. The monument itself consists of 112 gigantic stone blocks arranged in 3 overlapping circles.",
                    coverimage: "https://www.melivecode.com/attractions/7.jpg"
                },
                {
                    id: 8,
                    name: "Statue of Liberty",
                    detail: "The Statue of Liberty is a colossal neoclassical sculpture on Liberty Island in New York Harbor in New York City, in the United States. The copper statue, a gift from the people of France to the people of the United States.",
                    coverimage: "https://www.melivecode.com/attractions/8.jpg"
                },
                {
                    id: 9,
                    name: "Sydney Opera House",
                    detail: "The Sydney Opera House is a multi-venue performing arts centre in Sydney. Located on the banks of the Sydney Harbour, it is often regarded as one of the most famous and distinctive buildings and a masterpiece of 20th century architecture.",
                    coverimage: "https://www.melivecode.com/attractions/9.jpg"
                },
                {
                    id: 10,
                    name: "Great Pyramid of Giza",
                    detail: "The Great Pyramid of Giza is the oldest and largest of the pyramids in the Giza pyramid complex bordering present-day Giza in Greater Cairo, Egypt. It is the oldest of the Seven Wonders of the Ancient World, and the only one to remain largely intact.",
                    coverimage: "https://www.melivecode.com/attractions/10.jpg"
                },
                {
                    id: 11,
                    name: "Hollywood Sign",
                    detail: "The Hollywood Sign is an American landmark and cultural icon overlooking Hollywood, Los Angeles, California. It is situated on Mount Lee, in the Beachwood Canyon area of the Santa Monica Mountains. Spelling out the word Hollywood in 45 ft (13.7 m)-tall white capital letters and 350 feet (106.7 m) long.",
                    coverimage: "https://www.melivecode.com/attractions/11.jpg"
                },
                {
                    id: 12,
                    name: "Wat Phra Kaew",
                    detail: "Wat Phra Kaew, commonly known in English as the Temple of the Emerald Buddha and officially as Wat Phra Si Rattana Satsadaram, is regarded as the most sacred Buddhist temple in Thailand. The complex consists of a number of buildings within the precincts of the Grand Palace in the historical centre of Bangkok.",
                    coverimage: "https://www.melivecode.com/attractions/12.jpg"
                }
            ],
        }
    },

}
</script>

<style>

</style>