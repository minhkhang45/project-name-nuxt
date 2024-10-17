<template>

  <div>
    <NuxtRouteAnnouncer />
    <div class="flex mx-[auto]  justify-between h-[70px] max-w-[1296px]">
      <img src="https://templatemo.com/templates/templatemo_576_snapx_photography/assets/images/logo.png" alt="logo"
        class="max-w-[142px] max-h-[54px] my-auto">
      <div class="bg-[#00bdfe] w-[620px] flex justify-evenly text-white items-center">
        <NuxtLink to="/" class="">HOME</NuxtLink>
        <NuxtLink class="">PHOTOS & VIDEOS</NuxtLink>
        <NuxtLink to="/cayegor" class="">CATEGORIES</NuxtLink>
        <NuxtLink class="">USERS</NuxtLink>
      </div>
      <button
        class="transition duration-300 border-[#00bdfe] border hover:bg-[#00bdfe] hover:text-white rounded-xl px-[30px] py-[10px] my-auto h-fit text-[#00bdfe] flex items-center font-bold">
        <Icon name="mdi:account" class="text-xl" /> Sign In/Up
      </button>

    </div>
    <NuxtPage></NuxtPage>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');

body {
  font-family: "Roboto", sans-serif;
  font-weight: 400;
  font-style: normal;
}

.roboto-thin {
  font-family: "Roboto", sans-serif;
  font-weight: 100;
  font-style: normal;
}

.roboto-light {
  font-family: "Roboto", sans-serif;
  font-weight: 300;
  font-style: normal;
}

.roboto-regular {
  font-family: "Roboto", sans-serif;
  font-weight: 400;
  font-style: normal;
}

.roboto-medium {
  font-family: "Roboto", sans-serif;
  font-weight: 500;
  font-style: normal;
}

.roboto-bold {
  font-family: "Roboto", sans-serif;
  font-weight: 700;
  font-style: normal;
}

.roboto-black {
  font-family: "Roboto", sans-serif;
  font-weight: 900;
  font-style: normal;
}

.roboto-thin-italic {
  font-family: "Roboto", sans-serif;
  font-weight: 100;
  font-style: italic;
}

.roboto-light-italic {
  font-family: "Roboto", sans-serif;
  font-weight: 300;
  font-style: italic;
}

.roboto-regular-italic {
  font-family: "Roboto", sans-serif;
  font-weight: 400;
  font-style: italic;
}

.roboto-medium-italic {
  font-family: "Roboto", sans-serif;
  font-weight: 500;
  font-style: italic;
}

.roboto-bold-italic {
  font-family: "Roboto", sans-serif;
  font-weight: 700;
  font-style: italic;
}

.roboto-black-italic {
  font-family: "Roboto", sans-serif;
  font-weight: 900;
  font-style: italic;
}
</style>