<template>
    <div class="max-w-7xl mx-auto grid grid-cols-4 gap-4">
        <div class="main-left col-span-2">
        <div class="p-12 bg-white border border-gray-200 rounded-lg">
            <h1 class="mb-6 text-2xl">Signup now</h1>
            <p class="mb-6 text-gray-500">
                            Lorem ipsum dolor sit mate. Lorem ipsum dolor sit mate. Lorem ipsum dolor sit mate.
                            Lorem ipsum dolor sit mate. Lorem ipsum dolor sit mate. Lorem ipsum dolor sit mate.
                        </p>
    <p class="font-bold">
    Already have an account? <RouterLink to = "/login" class="underline">Click here</RouterLink> to login instant!
    </p>
        </div>
        </div>
        <div class="main-center col-span-2 space-y-4">
        <div class="p-12 bg-white border border-gray-200 rounded-lg">
            <form @submit.prevent="createUser" class="space-y-6">

                           <div>
                                <label>Name</label><br>
                                <input type="text" placeholder="Your name" class="w-full mt-2 py-4 px-6 border border-gray-200 rounded-lg" v-model="name">
                            </div>
                            <div>
                                <label>Last Name</label><br>
                                <input type="text" placeholder="Your Last name" class="w-full mt-2 py-4 px-6 border border-gray-200 rounded-lg" v-model="lastname">
                            </div>

                            <div>
                                <label for="email">E-mail</label><br>
                                <input type="email" placeholder="Your e-mail address" class="w-full mt-2 py-4 px-6 border border-gray-200 rounded-lg" v-model="email">
                            </div>

                            <div>
                                <label>Password</label><br>
                                <input type="password" placeholder="Your password" class="w-full mt-2 py-4 px-6 border border-gray-200 rounded-lg"  v-model="password" required>
                            </div>

                            <div>
                                <label>Repeat password</label><br>
                                <input type="password" placeholder="Repeat your password" class="w-full mt-2 py-4 px-6 border border-gray-200 rounded-lg">
                            </div>

                            <div>
                                <button class="py-4 px-6 bg-purple-600 text-white rounded-lg">Signup</button>
                            </div>
                        </form>
        </div>
    </div>
    </div>
</template>

<script>

export default {
  data() {
    return {
      name:'',
      lastname:'',
      email: '',
      password: ''
    };
  },
  methods: {
    createUser() {
      const user = {
        name: this.name,
        lastName: this.lastname,
        email: this.email,
        password: this.password
      };

      // تخزين بيانات المستخدم في LocalStorage
      localStorage.setItem('email', JSON.stringify(user));
      alert('User created and saved to LocalStorage!');
    }
  }
};
</script>