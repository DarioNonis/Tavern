<template>
    <div class="mb-3">
        <label for="WebHookUrl" class="form-label">{{ $t("WebHookUrl") }}<span style="color: red;"><sup>*</sup></span></label>
        <input id="WebHookUrl" v-model="$parent.notification.webHookUrl" type="text" class="form-control" required>

        <label for="secretKey" class="form-label">{{ $t("SecretKey") }}<span style="color: red;"><sup>*</sup></span></label>
        <input id="secretKey" v-model="$parent.notification.secretKey" type="text" class="form-control" required>

        <div class="form-text">
            <p>For safety, must use secret key</p>
            <i18n-t tag="p" keypath="Read more:">
                <a href="https://developers.dingtalk.com/document/robots/custom-robot-access" target="_blank">https://developers.dingtalk.com/document/robots/custom-robot-access</a>
            </i18n-t>
        </div>
    </div>
</template>
