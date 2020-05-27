<template>
    <div>
        <CRow>
            <CCol md="2"></CCol>
            <CCol md="8">
                <CRow>
                    <CCol>
                        <div class="banner-text">
                            <h1>Ethereum's</h1>
                            <h1>Original Wallet</h1>
                            <p>MyEtherWallet (our friends call us MEW) is a free, client-side interface helping you interact with the Ethereum blockchain. Our easy-to-use, open-source platform allows you to generate wallets, interact with smart contracts, and so much more.</p>
                        </div>
                    </CCol>
                    <CCol>
                        <img style="height:400px; width: 450px;" src="img/banner-image.png"/>
                    </CCol>
                </CRow>
                <CRow>
                    <CCol lg="6" style="margin-bottom:5px;">
                        <div style="height:300px; background-color: #5a78f0; padding: 70px 20px 5px; border-radius: 10px; cursor:pointer" @click="createAccount()">
                            <div style="hegiht:100%;">
                                <div>
                                    <p style="color: white;font-size:20px;">Create A New Vallet</p>
                                    <p style="color: white;margin-top:10px;"> Generate your own unique Ethereum wallet. Receive a public address (0x...) and choose a method for access and recovery. </p>
                                </div>
                            </div>
                        </div>
                    </CCol>
                    <CCol lg="6" >
                        <div style="height:300px; background-color: #05c0a5; padding: 70px 20px 5px;border-radius: 10px; cursor: pointer">
                             <div style="hegiht:100%;">
                                <div>
                                    <p style="color: white;font-size:20px;">Acccess My Vallet</p>
                                    <p style="color: white;margin-top:10px;"> Generate your own unique Ethereum wallet. Receive a public address (0x...) and choose a method for access and recovery. </p>
                                </div>
                            </div>
                        </div>
                    </CCol>
                </CRow>
            </CCol>
            <CCol md="2"></CCol>
        </CRow>
    </div>
</template>

<script>
export default {
    name: "HomePage",
    methods: {
        createAccount() {
            this.$router.push({path:'/account/create'})
        }
    }
}
</script>

<style scoped>

    .banner-text h1 {
        color: #003945;
        font-weight:bold;

    }
    .banner-text p {
        line-height: 21px;
    }

    .banner-image img {
       
        height: 252px;
        margin: 0 0 0 auto;
        width: 400px;
    }

</style>
