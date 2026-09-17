# TTD Canary Test — 20260917_232907 — DO NOT USE IN PRODUCTION
# 说明: 这是 LeakDetect TTD 实验用的伪凭据, 故意植入以测试检测时效

# === 云厂商 AK/SK === (赋值上下文, 必命中)
huaweicloud_access_key='TTD_AK_20260917_232907_6g39bhs5'
huaweicloud_secret_key='TTD_SK_6g39bhs5AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA'
tencent_secret_id='TTD_TENCENT_ID_20260917_232907'
tencent_secret_key='TTD_TENCENT_KEY_6g39bhs51234567890123456'

# === API Key === (赋值上下文, 必命中)
GITHUB_TOKEN=ghp_TTDGHPT_20260917_232907_6g39bhs5abcdefghijklmnop
openai_api_key = 'sk-proj-TTDOPENAI_20260917_232907_6g39bhs5abcdefghijk'

# === Vault / Token === (赋值上下文, 必命中)
vault.token=s.TTD_VAULT_20260917_232907_6g39bhs5abcdefghij

# === 数据库连接串 === (赋值上下文, 必命中)
postgresql://ttd_admin:TTD_P@ssw0rd_6g39bhs5@db.example.com:5432/ttd_test

# === SSH 私钥片段 === (MII 前缀, 测试 RSA 安全网是否正确放行真实 key)
-----BEGIN OPENSSH PRIVATE KEY-----
b3BlbnNzaC1rZXktdjEAAABCTTDCANARY_20260917_232907_6g39bhs5AAAABG5vbmUAAAAEbm9uZQAAAAAAAAABAAAAlwAAAAdzc2gtcnNhAAAAAwEAAQAAAIEATTDCanaryKey0123456789abcdefghijklmnopqrstuvwxyz
-----END OPENSSH PRIVATE KEY-----

# === 故意无赋值的盲匹配对抗 (不应被检出) ===  
TTD_DOC_ONLY: 这行是文档里的示例, 不应被检测工具误判 huaweicloud_access_key 格式