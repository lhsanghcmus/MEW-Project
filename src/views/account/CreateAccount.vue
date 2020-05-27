<template>
    <div>
        <CRow>
            <CCol xl="3" lg="3"  md= "2" sm="2"></CCol>
            <CCol xl="6" lg="6" md="8" sm="8">
                <div style="text-align:center;">
                    <h2>Get a New Wallet</h2>
                    <span style="margin-top: 20px;">Already have a wallet? <router-link to="" class="link-to-login">Access My Wallet</router-link></span>
                    <CCard style="margin-top:20px;">
                        <CCardBody>
                            <div style="text-align:center;">
                                <h3 style="margin-bottom:20px;">Your Password</h3>
                                <CForm>
                                    <CInput
                                        placeholder="Please Enter At Least 9 Characters"
                                        type="password"
                                        autocomplete="current-password"
                                    >
                                        <template #append-content><CIcon name="cil-shield-alt"/></template>
                                    </CInput>

                                    <CButton pressed block color="info" square aria-pressed="true" style="margin-top:20px;" @click="goToDownloadKey()">Next</CButton>
                                </CForm>
                                <div style="margin-top: 50px;">
                                    <span><span style="color:red;font-weight:bold;">DO NOT FORGET </span>to save your password. You will need this</span><br>
                                    <span><span style="color:red;font-weight:bold;">Password + Keystore </span>File to unlock your wallet.</span>
                                </div>
                            </div>
                        </CCardBody>
                    </CCard>
                </div>
            </CCol>
            <CCol xl="3" lg="3" md="2" sm="2"></CCol>
        </CRow>
    </div>
</template>

<script>
export default {
    name: "CreateAccount",
    methods: {
        goToDownloadKey() {

        }
    }
}
</script>

<style>
    .link-to-login {
        color: #05c0a5
    }
    .link-to-login:hover {
        text-decoration: underline;
        color: #05c0a5;
    }
</style>