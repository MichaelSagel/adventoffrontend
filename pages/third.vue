<template>
  <div class="third">
      <button
        class="firstWhiteKey yellow"
        @click="playSound(sound1)"
      ></button>
      <button
        class="secondWhiteKey yellow"
        @click="playSound(sound2)"
      ></button>
      <button
        class="thirdWhiteKey yellow"
        @click="playSound(sound3)"
      ></button>
      <button 
        class="fourthWhiteKey yellow"
        @click="playSound(sound4)"
      ></button>
      <button
        class="fifthWhiteKey yellow"
        @click="playSound(sound5)"
      ></button>
      <button 
        class="sixthWhiteKey yellow"
        @click="playSound(sound6)"
      ></button>
      <button
        class="seventhWhiteKey yellow"
        @click="playSound(sound7)"
      ></button>
      <button
        class="eighthWhiteKey yellow"
        @click="playSound(sound8)"
      ></button>
      <button
        class="ninthWhiteKey yellow"
        @click="playSound(sound9)"
      ></button>
      <button
        class="tenthWhiteKey yellow"
        @click="playSound(sound10)"
      ></button>
      <button
        class="eleventhWhiteKey yellow"
        @click="playSound(sound11)"
      ></button>
      <button
        class="twelfthWhiteKey yellow"
        @click="playSound(sound12)"
      ></button>
      <button
        class="thirteenthWhiteKey yellow"
        @click="playSound(sound13)"
      ></button>
      <button
        class="firstBlackKey pink"
        @click="playSound(sound14)"
      ></button>
      <button
        class="secondBlackKey pink"
        @click="playSound(sound15)"
      ></button>
      <button 
        class="thirdBlackKey pink"
        @click="playSound(sound16)"
      ></button>
      <button
        class="fourthBlackKey pink"
        @click="playSound(sound17)"
      ></button>
      <button
        class="fifthBlackKey pink"
        @click="playSound(sound18)"
      ></button>
      <button
        class="sixthBlackKey pink"
        @click="playSound(sound19)"
      ></button>
      <button
        class="seventhBlackKey pink"
        @click="playSound(sound20)"
      ></button>
      <button
        class="eighthBlackKey pink"
        @click="playSound(sound21)"
      ></button>
      <button
        class="ninthBlackKey pink"
        @click="playSound(sound22)"
      ></button>
      <button
        class="tenthBlackKey pink"
        @click="playSound(sound23)"
      ></button>
  </div>
</template>

<script>
import sound1 from "@/assets/audio/key-1.mp3";
import sound2  from "@/assets/audio/key-2.mp3";
import sound3  from "@/assets/audio/key-3.mp3";
import sound4  from "@/assets/audio/key-4.mp3";
import sound5  from "@/assets/audio/key-5.mp3";
import sound6  from "@/assets/audio/key-6.mp3";
import sound7  from "@/assets/audio/key-7.mp3";
import sound8  from "@/assets/audio/key-8.mp3";
import sound9  from "@/assets/audio/key-9.mp3";
import sound10  from "@/assets/audio/key-10.mp3";
import sound11  from "@/assets/audio/key-11.mp3";
import sound12  from "@/assets/audio/key-12.mp3";
import sound13  from "@/assets/audio/key-13.mp3";
import sound14  from "@/assets/audio/key-14.mp3";
import sound15  from "@/assets/audio/key-15.mp3";
import sound16  from "@/assets/audio/key-16.mp3";
import sound17  from "@/assets/audio/key-17.mp3";
import sound18  from "@/assets/audio/key-18.mp3";
import sound19  from "@/assets/audio/key-19.mp3";
import sound20  from "@/assets/audio/key-20.mp3";
import sound21  from "@/assets/audio/key-21.mp3";
import sound22  from "@/assets/audio/key-22.mp3";
import sound23  from "@/assets/audio/key-23.mp3";
export default {
  colorMode: "third",
  data() {
    return {
      sound1,
      sound2,
      sound3,
      sound4,
      sound5,
      sound6,
      sound7,
      sound8,
      sound9,
      sound10,
      sound11,
      sound12,
      sound13,
      sound14,
      sound15,
      sound16,
      sound17,
      sound18,
      sound19,
      sound20,
      sound21,
      sound22,
      sound23,
    };
  },
   methods: {
    playSound(sound) {
      let audio = new Audio(sound);
      audio.play();
    },
  },
};
</script>

<style scoped lang="scss">
@import "./../assets/styles/third.scss";
</style>