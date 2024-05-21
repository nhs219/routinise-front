<template>
  <nav class="navbar navbar-expand-sm border-bottom">
    <div class="container-fluid">
      <a class="navbar-brand fw-bold" href="/index.html">Routinise</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarScroll" aria-controls="navbarScroll" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarScroll">
        <ul class="navbar-nav me-auto navbar-nav-scroll" style="--bs-scroll-height: 100px;">
        </ul>
        <ul class="navbar-nav flex-row">
          <li class="dropdown">
            <a class="btn dropdown-toggle" href="#" role="button" id="dropdownMenuLink" data-bs-toggle="dropdown" aria-expanded="false">
              <img class="profile-image" src="@/assets/img/profile.png" alt="image">
            </a>
            <ul class="dropdown-menu dropdown-menu-end" aria-labelledby="dropdownMenuLink">
              <li><a class="dropdown-item" href="#"><i class="bi bi-star"></i> 내 정보</a></li>
              <li><a class="dropdown-item" href="#"><i class="bi bi-gear-wide"></i> 설정</a></li>
              <li><hr class="dropdown-divider"></li>
              <li><a class="dropdown-item" href="#"><i class="bi bi-box-arrow-right"></i> 로그아웃</a></li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "TheNav"
}
</script>

<style scoped>
  .profile-image {
    width: 40px;
    height: 40px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .dropdown-toggle::after {
    display: none;
  }
</style>