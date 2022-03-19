<template>
  <div class="fifth">
    <img src="../assets/images/fifth/podcast-cover.png" />
    <div class="fifth_content">
      <div class="content__test">Listen to all the Compressed.fm Episodes</div>
      <div class="content__list" v-for="item in list" :key="item.id">
        <template v-if="!item.clicked">
          <button
            class="content__btn"
            @click="
              (item.clicked = true), clicked_function(item.id, item.clicked)
            "
          >
            <img
              class="content__checkbox"
              src="../assets/images/fifth/checkbox--unchecked.svg"
            />
            {{ item.id }} || {{ item.name }}
          </button>
        </template>
        <template v-else>
          <button class="content-clicked__btn" @click="item.clicked = false">
            <img
              class="content__checkbox"
              src="../assets/images/fifth/checkbox--checked.svg"
            />
            {{ item.id }} || {{ item.name }}
          </button>
        </template>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  colorMode: "fifth",
   beforeMount() {
    document.addEventListener("keydown", this.shift_pressed);
    document.addEventListener("keyup", this.shift_released);
    document.addEventListener("mouseup", this.mouse_click);
  },
  destroyed() {
    document.removeEventListener("keydown", this.shift_pressed);
    document.removeEventListener("keyup", this.shift_released);
    document.removeEventListener("mouseup", this.mouse_click);
  },
  data: function () {
    return {
      shift_condition: false,
      shift_code_left: "ShiftLeft",
      shift_code_right: "ShiftRight",
      list: [
        {
          id: 1,
          name: "James Q Quick's Origin Story",
          clicked: false,
        },
        {
          id: 2,
          name: "Amy Dutton's Origin Story",
          clicked: false,
        },
        {
          id: 3,
          name: "The Tech Behind Compressed.fm",
          clicked: false,
        },
        {
          id: 4,
          name: "Starting a New Development Project",
          clicked: false,
        },
        {
          id: 5,
          name: "How Do you Start a New Design Project?",
          clicked: false,
        },
        {
          id: 6,
          name: "Freelancing (Part 1)",
          clicked: false,
        },
        {
          id: 7,
          name: "Freelancing (Part 2)",
          clicked: false,
        },
        {
          id: 8,
          name: "The Tech Behind jamesqquick.com",
          clicked: false,
        },
        {
          id: 9,
          name: "Teh Tech Behind SelfTeach.me",
          clicked: false,
        },
        {
          id: 10,
          name: "Design Fundamentals (Part 1)",
          clicked: false,
        },
        {
          id: 11,
          name: "Design Fundamentals (Part 2)",
          clicked: false,
        },
        {
          id: 12,
          name: "Productivity: Tools, Tips, and Workflows",
          clicked: false,
        },
        {
          id: 13,
          name: "The Future of Code with No Code",
          clicked: false,
        },
        {
          id: 14,
          name: "Building the Perfect Desk Setup",
          clicked: false,
        },
        {
          id: 15,
          name: "Everything You Need to Know to Get Started in SvelteKit",
          clicked: false,
        },
        {
          id: 16,
          name: "Live Streaming for Beginners",
          clicked: false,
        },
        {
          id: 17,
          name: "All Things Automated",
          clicked: false,
        },
        {
          id: 18,
          name: "Amy Gives James a Design Consult",
          clicked: false,
        },
        {
          id: 19,
          name: "Figma for Everyone",
          clicked: false,
        },
        {
          id: 20,
          name: "Learning and Building in Public",
          clicked: false,
        },
        {
          id: 21,
          name: "Getting Your First Dev Job",
          clicked: false,
        },
        {
          id: 22,
          name: "Hiring a Designer or Getting Your First UI / UX Job",
          clicked: false,
        },
        {
          id: 23,
          name: "IRL Freelance Proposal",
          clicked: false,
        },
        {
          id: 24,
          name: "Getting Started on YouTube",
          clicked: false,
        },
        {
          id: 25,
          name: "Starting your own Podcast",
          clicked: false,
        },
        {
          id: 26,
          name: "How Blogging Can Change Your Career",
          clicked: false,
        },
        {
          id: 27,
          name: "Talking to Some of Our Favorite Content Creators",
          clicked: false,
        },
        {
          id: 28,
          name: "Our Favorite Things: A Crossover Episode with Web Dev Weekly",
          clicked: false,
        },
        {
          id: 29,
          name: "Freelancing IRL: Unveiling a Site Redesign",
          clicked: false,
        },
        {
          id: 30,
          name: "Wordpress in 2021",
          clicked: false,
        },
        {
          id: 31,
          name: "Struggle Bus",
          clicked: false,
        },
        {
          id: 32,
          name: "Getting Started with TypeScript",
          clicked: false,
        },
        {
          id: 33,
          name: "Small Design Tweaks that Make All the Difference",
          clicked: false,
        },
        {
          id: 34,
          name: "Getting git",
          clicked: false,
        },
        {
          id: 35,
          name: "Crossover Episode with Purrfect Dev",
          clicked: false,
        },
        {
          id: 36,
          name: "SVGs FTW",
          clicked: false,
        },
        {
          id: 37,
          name: "Building a Course",
          clicked: false,
        },
      ],
    };
  },
  methods: {
    clicked_function: function (list_id, list_clicked) {
      if (list_clicked === false) {
        const podcast = this.list.find(function (element) {
          return element.id === list_id;
        });
        podcast.clicked = !podcast.clicked;
      }
    },
    shift_pressed: function(shift_pressed){
      if (shift_pressed.code === this.shift_code_left || shift_pressed.code === this.shift_code_right){
      console.log("down");
      this.shift_condition = !this.shift_condition;
      console.log(this.shift_condition);
      }
    },
    shift_released: function(shift_released){
      if (shift_released.code === this.shift_code_left || shift_released.code === this.shift_code_right){
      console.log("up");
      this.shift_condition = !this.shift_condition;
      console.log(this.shift_condition);
      }
    },
    mouse_click: function () {
      if(this.shift_condition === true){
        for (; this.item.id > 0; this.item.id--){
          this.item.clicked = true;
        }
      }
    },
  },
};
</script>
<style>
@import "./../assets/styles/fifth.css";
</style>