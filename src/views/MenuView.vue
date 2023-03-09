<template>
  <div class="menu-page">
    <h1>Our Menu</h1>
    <ul>
      <li v-for="(group, section) in groupedMenuItems" :key="section">
        <h2 class="section-header">{{ section }}</h2>
        <ul class="menu-items-container">
          <li v-for="item in group" :key="item.name" class="menu-item">
            <img :src="item.photo" :alt="item.name" />
            <div class="menu-item-details">
              <h3>{{ item.name }}</h3>
              <p>{{ item.description }}</p>
              <p class="price">{{ item.price }}</p>
            </div>
          </li>
        </ul>
      </li>
    </ul>
  </div>
</template>

<script>
import menuData from "@/menu.json";

export default {
  name: "MenuPage",
  data() {
    return {
      menuItems: menuData,
    };
  },
  computed: {
    groupedMenuItems() {
      return this.menuItems.reduce((groups, item) => {
        const group = groups[item.section] || [];
        group.push(item);
        groups[item.section] = group;
        return groups;
      }, {});
    },
  },
};
</script>

<style>
.menu-page {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100%;
}

ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

.menu-items-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.menu-item {
  margin: 20px;
  max-width: calc(100% / 3 - 20px);
  text-align: center;
}

img {
  width: 100%;
  max-width: 300px;
  height: auto;
  margin-bottom: 10px;
}

.section-header {
  margin: 20px 0;
}
</style>
