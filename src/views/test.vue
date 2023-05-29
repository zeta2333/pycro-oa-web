<template>
  <div>
    <div>账号切换</div>
    <!-- <button @click="wjl()" type="default" size="mini">王经理</button> -->
    <button @click="admin()" type="default" size="mini">管理员</button>
    <button @click="zhangsan()" type="default" size="mini">张三</button>
    <button @click="lisi()" type="default" size="mini">李四</button>
    <div>当前token：{{ token }}</div>
  </div>
</template>

<script>
export default {
  name: "Test",

  data() {
    return {
      token: "",
    };
  },

  created() {
    this.token = window.localStorage.getItem("token");
  },

  methods: {
    admin() {
      window.localStorage.setItem("token", "");
      let token =
        "eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNLMwMzc2NjYz11EqLU4t8kwBikGYeYm5qUAtiSm5mXlKtQBwMnyHQgAAAA._utPtG_e9EJh38iWWFzJEqY7dhkIll_twXrLqWWziW_0XhQV7yX-oCibxV38FjfT8v5NU7f101nEnxwOR5GO-g";
      window.localStorage.setItem("token", token);
      this.token = window.localStorage.getItem("token");
    },

    zhangsan() {
      window.localStorage.setItem("token", "");
      let token =
        "eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNLMwMzc2NTC21FEqLU4t8kxRsjKHMPMSc1OBWqoyEvPSixPzlGoB_LLDnUUAAAA.fXIxUz4WZTarrCGNAQYfw0yt8q-0dX5lalmR3-qOPW7BtBZDPrlmILVXYEDNyVIHqTNeNoi4nkugyNgMFfV4qQ";
      window.localStorage.setItem("token", token);
      this.token = window.localStorage.getItem("token");
    },
    lisi() {
      window.localStorage.setItem("token", "");
      let token =
        "eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNLMwMzc2NjE211EqLU4t8kxRsjKBMPMSc1OBWnIyizOVagEjVCwDQQAAAA.a6eWDCZIkKTUCV3UBrFM6VlTRXYbFs77t-GBas_PmBw4OC8LHQABVPigZITpe2FPaUKIE0llsTZZVLLWrhR8mQ";
      window.localStorage.setItem("token", token);
      this.token = window.localStorage.getItem("token");
    },

    zzjl() {
      window.localStorage.setItem("token", "");
      let token =
        "eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNDM3NjMwNLYw11EqLU4t8kxRsjKFMPMSc1OBWqqqsnKUagGHebUNQQAAAA.FcCkD6QfaP8bd_3MYsRD6Tp9wr9JSRFWIUuIdG5O7XxhIeyWfzGLp40_Lesx_kWMMaaskh_ba3NrTlj8-nP6OA";
      window.localStorage.setItem("token", token);
      this.token = window.localStorage.getItem("token");
    },
  },
};
</script>
