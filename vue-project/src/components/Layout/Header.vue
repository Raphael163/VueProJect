<template>
    <header class="bg-purple-900 text-white">
      <nav class="container mx-auto flex items-center justify-between py-4">
        <div>
          <a href="/" class="flex items-center space-x-2 text-xl font-bold">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 19l9 2-9-18-9 18 9-2zm0 0v-8"/>
            </svg>
            <span>Testing</span>
          </a>
        </div>
        <div>
          <ul class="flex space-x-4">
            <li>
              <a href="/about" class="hover:text-purple-300 transition duration-300">О нас</a>
            </li>
            <li>
              <router-link to="/contacts">Контакты</router-link>
            </li>
            <li>
              <a href="/login" class="hover:text-purple-300 transition duration-300">Личный кабинет</a>
            </li>
            <li>
              <a href="/cart" class="flex items-center hover:text-purple-300 transition duration-300">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 18h9a2 2 0 002-2V6a2 2 0 00-2-2H9a2 2 0 00-2 2v10a2 2 0 002 2zM6 6h0"/>
                </svg>
                <span>Корзина</span>
              </a>
            </li>
          </ul>
        </div>
      </nav>
    </header>
  </template>
  
  <style>
  header {
    background-color: #3f0e40;
    padding-top: 1rem;
    padding-bottom: 1rem;
  }
  
  a {
    padding-left: 0.5rem;
    padding-right: 0.5rem;
    border-radius: 0.25rem;
    transition-property: background-color, color;
    transition-duration: 300ms;
  }
  
  a:hover {
    background-color: #6b7280;
    color: #d1d5db;
  }
  
  svg {
    height: 1.5rem;
    width: 1.5rem;
  }
  </style>
  