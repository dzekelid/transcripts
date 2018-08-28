swagger: "2.0"
x-collection-name: LiveChat
x-complete: 1
info:
  title: LiveChat REST API
  description: -introductionwelcome-to-the-livechat-api-documentationour-api-provides-a-set-of-flexible-tools-which-you-can-use-to-create-new-outstanding-projects--we-smile-a-bit-more-each-time-we-see-skilled-developers-unleash-their-creativityplease-note-that-this-documentation-refers-to-the-latest-api-version-2-0--if-you-are-looking-for-the-previous-version-check-out-the-deprecated-api-1-0-documentation--basic-api-usageall-livechat-api-requests-start-with--httpsapi-livechatinc-com-please-note-that-all-livechat-api-requests-must-use-https-protocol-the-next-segment-of-the-url-path-depends-on-the-type-of-your-request--for-example-use--httpsapi-livechatinc-comagents--to-get-or-modify-the-agents-data-all-requests-must-have-xapiversion-header-set-to-the-number-of-the-version-that-youd-like-to-use--the-most-recent-version-is-2--authenticationtwo-common-authentication-methods-are-supported--oauth-2-0--and--api-key--oauth-2-0oauth-2-0-authentication-is-the-recommended-way-of-authenticating-to-livechat-api-it-is-the-most-secure-way-of-making-api-calls--with-this-flow-you-will-get-access-only-to-some-parts-of-livechat-account-such-as-reading-agents-list--this-is-more-secure-than--api-key-flowhttpsdocs-livechatinc-comrestapiapikey--which-has-always-access-to-all-livechat-account-data-to-start-using-oauth-2-0-please-read-a-dedicated--authorizationhttpsdocs-livechatinc-comauthorization--guide--api-keyif-you-want-to-build-a-private-app-that-will-run-on-your-own-server-you-can-skip-the-oauth-2-0-flow-and-use-the-api-key--please-note-this-flow-of-making-api-calls-is-less-secure-because-the-api-key-gives-access-to-all-livechat-account-data-with-this-authorization-method-you-will-need-to-include-your-livechat-login-and--api-key--for-each-method-call--youll-find-the-api-key-in--your-livechat-profilehttpsmy-livechatinc-comagentsapikey-authentication-to-the-api-occurs-via--http-basic-authhttpen-wikipedia-orgwikibasic-access-authentication--provide-your--login--as-the-basic-auth-username-and-the--api-key--as-the-password--you-must-authenticate-for-all-requests-all-api-requests-must-be-made-over-https--data-formatthe-livechat-api-returns-the-data-in-the--jsonhttpen-wikipedia-orgwikijson--format--check-out-the-following-example--jsonpall-requests-made-with-http-get-are--jsonphttpen-wikipedia-orgwikijsonpenabled--to-use-jsonp-append--callback--and-the-name-of-your-callback-function-to-the-request--error-handlingthe-errors-are-returned-using-the-standard-http-error-code-syntax--in-general-the-codes-in-the-2xx-range-indicate-success-the-codes-in-the-4xx-range-indicate-an-error-incorrect-or-missing-parameters-not-authenticated-etc--and-the-codes-in-the-5xx-range-indicate-an-error-with-the-livechat-servers--any-additional-info-is-included-in-the-body-of-the-return-call-jsonformatted--http-status-codes-summary---400---the-request-is-incorrect-please-make-sure-that-the-passed-arguments-are-matching-the-format-in-the-methods-documentation----401---unauthorized--you-attempt-to-authenticate-with-an-invalid-username-or-api-key----404---not-found--you-attempt-to-request-a-resource-which-doesnt-exist----500---internal-server-error--something-unexpected-happened-on-our-end--please-try-again-or-contact-our-support--crossdomainall-crossdomain-api-requests-made-by-a-web-browser-are-denied-for-security-reasons--it-means-that-the-browserbased-requests-are-not-allowed-from-3rd-party-domains-including--localhost--livechat-api-librariesall-api-calls-include-an-api-key-that-can-be-easily-stolen-when-making-a-request-using-a-web-browser--it-means-you-should-use-backend-languages-for-api-requests--here-is-a-list-of-the-readytouse-libraries---php-library-for-livechat-apihttpsgithub-comlivechatapiclientphp-hosted-on-github----node-js-library-for-livechat-apihttpsgithub-comlivechatapiclientnodejs-hosted-on-github----ruby-library-for-livechat-apihttpsgithub-comcxzlivechat-client-hosted-on-github----c-library-for-livechat-apihttpsgithub-comlivechatapiclientcsharp-hosted-on-github--external-livechat-api-libraries---r-library-for-livechat-apihttpsgithub-comlawwulivechatr-hosted-on-github-did-you-write-your-own-library-and-want-it-listed-here-let-us-know
  version: 1.0.0
host: api.livechatinc.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /chats/ABC123/send_transcript:
    post:
      summary: Send chat transcript to e-mail
      description: ""
      operationId: ChatsABC123SendTranscriptPost
      x-api-path-slug: chatsabc123send-transcript-post
      parameters:
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - Send
      - Chat
      - Transcript
      - To
      - E-mail