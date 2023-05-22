<template>
  <footer class="bg-light py-3">
    <div class="container">
      <div class="row">
        <div class="col-md-4">
          <h4>{{ title }}</h4>
          <p>{{ description }}</p>
        </div>
        <div class="col-md-4">
          <h4>{{ linksTitle }}</h4>
          <ul class="list-unstyled">
            <li><a href="#">Link 1</a></li>
            <li><a href="#">Link 2</a></li>
            <li><a href="#">Link 3</a></li>
          </ul>
        </div>
        <div class="col-md-4">
          <h4>{{ contactTitle }}</h4>
          <address>
            <strong>{{ address }}</strong
            ><br />
            {{ city }}, {{ state }} {{ zip }}<br />
            <abbr title="Phone">P:</abbr> {{ phone }}<br />
            <a href="mailto:{{ email }}">{{ email }}</a>
          </address>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooteR",
  data() {
    return {
      title: "Footer Title",
      description: "Footer description",
      linksTitle: "Links",
      contactTitle: "Contact Us",
      address: "1234 Main St.",
      city: "Anytown",
      state: "CA",
      zip: "12345",
      phone: "555-555-5555",
      email: "email@example.com",
    };
  },
};
</script>
