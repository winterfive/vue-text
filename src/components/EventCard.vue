<template>
  <div class="event-card -shadow">
    <span class="eyebrow">@{{ event.time }} on {{ event.date }}</span>
    <h4 class="title">{{ event.title }}</h4>
    <span>{{ event.attendees.length }} attending.</span>
  </div>
</template>

<script>
export default {
  data() {
    return {
      event: {
        id: 1,
        title: "Park Cleanup",
        date: "Tuesday Aug 4, 2019",
        time: "6:00",
        attendees: [{ id: "abc", name: "Adam" }, { id: "abcd", name: "Darwin" }]
      }
    };
  }
};
</script>

<style scoped>
h4 {
  color: green;
  border: 1px solid #ccc;
  padding-left: 10px;
}
</style>
