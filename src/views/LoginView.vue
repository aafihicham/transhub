<template>
    <div class="max-w-7xl mx-auto grid grid-cols-4 gap-4">
        <div class="main-left col-span-2">
        <div class="p-12 bg-white border border-gray-200 rounded-lg">
            <h1 class="mb-6 text-2xl">Login</h1>
            <p class="mb-6 text-gray-500">
                            Lorem ipsum dolor sit mate. Lorem ipsum dolor sit mate. Lorem ipsum dolor sit mate.
                            Lorem ipsum dolor sit mate. Lorem ipsum dolor sit mate. Lorem ipsum dolor sit mate.
                        </p>
    <p class="font-bold">
    You don't have an account? <RouterLink to ="/signup" class="underline">Click here</RouterLink> to signup!
    </p>
        </div>
        </div>
        <div class="main-center col-span-2 space-y-4">
        <div class="p-12 bg-white border border-gray-200 rounded-lg">
            <form class="space-y-6">


                            <div>
                                <label>E-mail</label><br>
                                <input type="email" placeholder="Your e-mail address" class="w-full mt-2 py-4 px-6 border border-gray-200 rounded-lg" v-model="email">
                            </div>

                            <div>
                                <label>Password</label><br>
                                <input type="password" placeholder="Your password" class="w-full mt-2 py-4 px-6 border border-gray-200 rounded-lg" v-model="password">
                            </div>

                            <div>
                                <button class="py-4 px-6 bg-purple-600 text-white rounded-lg" type="submit">Login</button>
                            </div>
                            <div v-if="loginError" class="error">{{ loginError }}</div>

                        </form>
        </div>
        </div>
    </div>
</template>

<script>

export default {
  data() {
    return {
      email: '',
      password: '',
      loginError: null,
    };
  },
  methods: {
    loginUser() {
      // استرجاع بيانات المستخدم من LocalStorage
      const savedUser = JSON.parse(localStorage.getItem('email'));

      if (savedUser) {
        // التحقق من صحة البيانات المدخلة
        if (
          this.email === savedUser.email &&
          this.password === savedUser.password
        ) {
          alert('Login successful!');
          this.loginError = null;

          // يمكنك توجيه المستخدم إلى صفحة أخرى بعد تسجيل الدخول
          this.$router.push('/feed');
        } else {
          this.loginError = 'Invalid username or password';
        }
      } else {
        this.loginError = 'No user found. Please register first.';
      }
    },
  },
};
</script>
