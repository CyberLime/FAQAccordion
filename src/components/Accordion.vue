<script setup>
  const faqs = [
    {question: "What is Frontend Mentor, and how will it help me?", answer: "Frontend Mentor offers realistic coding challenges to help developers improve their frontend coding skills with projects in HTML, CSS, and JavaScript. It's suitable for all levels and ideal for portfolio building."},
    {question: "Is Frontend Mentor free?", answer: "Yes, Frontend Mentor offers both free and premium coding challenges, with the free option providing access to a range of projects suitable for all skill levels."},
    {question: "Can I use Frontend Mentor projects in my portfolio?", answer: "Yes, you can use projects completed on Frontend Mentor in your portfolio. It's an excellent way to showcase your skills to potential employers!"},
    {question: "How can I get help if I'm stuck on a challenge?", answer: "The best place to get help is inside Frontend Mentor's Discord community. There's a help channel where you can ask questions and seek support from other community members."}
  ];
</script>

<template>
  <ul v-for:="faq in faqs">
    <li>
      <details>
        <summary>{{ faq.question }}</summary>
        <p>{{ faq.answer }}</p>
      </details>
    </li>
  </ul>
</template>

<style scoped>
  ul {
    list-style: none;
  }

  ul li {
    margin-top: 40px;
  }

  summary {
    display: flex;
    justify-content: space-between;
    align-items: center;
    list-style: none;
    font-weight: 600;
    width: 95%;
  }

  summary::after {
    content: '';
    width: 27px;
    height: 27px;
    background: url('../assets/images/icon-plus.svg') no-repeat;
    background-size: cover;
    transition: 0.2s;
  }

  details[open] > summary::after {
    width: 28px;
    height: 28px;
    background: url('../assets/images/icon-minus.svg') no-repeat;
  }

  summary::-webkit-details-marker {
    display: none;
  }
</style>