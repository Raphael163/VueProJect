<template>
    <div class="content">
      <div class="services">
        <div class="service" v-for="service in services" :key="service.id">
          <div class="service-icon">
            <i :class="service.icon"></i>
          </div>
          <div class="service-info">
            <h3>{{ service.title }}</h3>
            <p>{{ service.description }}</p>
            <p class="service-price">{{ service.price }}</p>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'Content',
    data() {
      return {
        services: [
          {
            id: 1,
            icon: 'fas fa-tools',
            title: 'Ремонт стиральных машин',
            description: 'Мы предоставляем качественный ремонт стиральных машин всех моделей и марок.',
            price: 'Цена: от $50',
          },
          {
            id: 2,
            icon: 'fas fa-laptop',
            title: 'Ремонт ноутбуков',
            description: 'Наши специалисты осуществляют ремонт ноутбуков с любыми проблемами и поломками.',
            price: 'Цена: от $80',
          },
          {
            id: 3,
            icon: 'fas fa-tv',
            title: 'Ремонт телевизоров',
            description: 'Мы производим ремонт телевизоров разных типов и размеров с высоким качеством работы.',
            price: 'Цена: от $100',
          },
          {
            id: 3,
            icon: 'fas fa-tv',
            title: 'Ремонт Видеокарт',
            description: 'Мы производим ремонт Видеокарт разных типов и размеров с высоким качеством работы.',
            price: 'Цена: от $110',
          },
          {
            id: 3,
            icon: 'fas fa-tv',
            title: 'Ремонт Планешетов',
            description: 'Мы производим ремонт Планешетов разных типов и размеров с высоким качеством работы.',
            price: 'Цена: от $100',
          },
          {
            id: 3,
            icon: 'fas fa-tv',
            title: 'Ремонт Телефонов',
            description: 'Мы производим ремонт Телефонов разных типов и размеров с высоким качеством работы.',
            price: 'Цена: от $120',
          },
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  .content {
    padding: 50px;
    text-align: center;
    background-color: white;
  }
  
  .services {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
  
  .service {
    width: 300px;
    margin: 20px;
    padding: 20px;
    background-color: #f5f5f5;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s;
  }
  
  .service:hover {
    transform: translateY(-5px);
  }
  
  .service-icon {
    font-size: 36px;
    margin-bottom: 10px;
  }
  
  .service-info h3 {
    margin-bottom: 10px;
  }
  
  .service-price {
    font-weight: bold;
  }
  
  .fa-tools,
  .fa-laptop,
  .fa-tv {
    color: #007bff;
  }
  </style>