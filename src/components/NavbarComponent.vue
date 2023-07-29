<script setup>
import { Navbar, NavbarLogo, NavbarCollapse, NavbarLink } from 'flowbite-vue'
</script>
<template>
    <Navbar>
      <template #logo>
        <NavbarLogo link="" alt="" image-url="">
          <p style="font-style: italic; color: black;">Fortopolio </p>
        </NavbarLogo>
      </template>
      <template #default="{isShowMenu}">
        <NavbarCollapse :isShowMenu="isShowMenu">
          <NavbarLink isActive link="#" class="hover:underline">Beranda</NavbarLink>
          <NavbarLink link="#" class="hover:underline">Tentang</NavbarLink>
          <NavbarLink link="https://wa.me/081224181451" class="hover:underline">Kontak</NavbarLink>
        </NavbarCollapse>
      </template>
    </Navbar>
</template>