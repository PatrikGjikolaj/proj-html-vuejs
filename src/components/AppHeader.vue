<script>

export default {
  data() {
    return {
      linksHeader: [
        {
          name: "Home",
          links: ["Start Here", "Succes Story", "About me", "About us 01", "About us 02", "About us 03", "Contact me", "Contact us", "Purchase Guide",
            "Privacy Policy", "Terms of Service"],
        },
        {
          name: "Pages",
          links: ["Start Here", "Succes Story", "About me", "About us 01", "About us 02", "About us 03", "Contact me", "Contact us", "Purchase Guide",
            "Privacy Policy", "Terms of Service"],
        },
        {
          name: "Courses",
          links: ["Start Here", "Succes Story", "About me", "About us 01", "About us 02", "About us 03", "Contact me", "Contact us", "Purchase Guide",
            "Privacy Policy", "Terms of Service"],
        },
        {
          name: "Features",
          links: ["Start Here", "Succes Story", "About me", "About us 01", "About us 02", "About us 03", "Contact me", "Contact us", "Purchase Guide",
            "Privacy Policy", "Terms of Service"],
        },
        {
          name: "Blog",
          links: ["Start Here", "Succes Story", "About me", "About us 01", "About us 02", "About us 03", "Contact me", "Contact us", "Purchase Guide",
            "Privacy Policy", "Terms of Service"],
        },
        {
          name: "Shop",
          links: ["Start Here", "Succes Story", "About me", "About us 01", "About us 02", "About us 03", "Contact me", "Contact us", "Purchase Guide",
            "Privacy Policy", "Terms of Service"],
        },
      ],
      blogInfo: ["Became a Better Blogger: Content Planning", "Promoting Your Online Business on Pinterest", "Gamification and Game-Based Learning", "Designs an Online Course from Expert's Perspective", "Why Online Courses Are the Future of Education"]
    }
  },
}
</script>

<template>
  <div class="container-fluid border-bottom">
    <div class="container">
      <nav class="navbar navbar-expand-lg bg-light row">
        <div class="col-2">
          <a class="navbar-brand" href=""><img src="../assets/dark-logo.png" alt="" class="img-fluid"></a>
        </div>
        <div class="col-10 d-flex justify-content-end">
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav ms-auto mb-2 mb-md-0">
              <template v-for="element in linksHeader">
                <li class="nav-item dropdown">
                  <a class="nav-link dropdown-toggle" href="" role="button" data-bs-toggle="dropdown"
                    aria-expanded="false">
                    {{ element.name }}
                  </a>
                  <ul class="dropdown-menu">
                    <template v-for="link in element.links">
                      <li><a class="dropdown-item" href="">{{ link }}</a></li>
                    </template>
                  </ul>
                </li>
              </template>
            </ul>
            <form role="search">
              <div class="input-group">
                <input type="text" class="form-control" placeholder="Search..." aria-label="Recipient's username"
                  aria-describedby="basic-addon2">
                <a class="input-group-text" id="basic-addon2">&#x1F50D;</a>
              </div>
            </form>
          </div>
        </div>
      </nav>
    </div>
  </div>
</template>

<style scoped>
a {
  text-decoration: none;
}
</style>
