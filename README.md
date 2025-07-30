# base85url
Это улучшенная альтернатива Base64url

# Пример
Этот пример текста ровно в сто символов длиной для демонстрации кодирования в base64url и base85url.

Base64url: 
```
0K3RgtC-0YIg0L_RgNC40LzQtdGAINGC0LXQutGB0YLQsCDRgNC-0LLQvdC-INCyINGB0YLQviDRgdC40LzQstC-0LvQvtCyINC00LvQuNC90L7QuSDQtNC70Y8g0LTQtdC80L7QvdGB0YLRgNCw0YbQuNC4INC60L7QtNC40YDQvtCy0LDQvdC40Y8g0LIgYmFzZTY0dXJsINC4IGJhc2U4NXVybC4=
```
*224 символа*

Base85url: 
```
CWR9X.MbxiA6W6If.~BUl7wd*pukqAlAWWy-aeOog4cLAi0)JuAzXRTDY4oyYde05abBiMfVbqDhJXqzpMuCA32l*HHcyUek0ZVDlv3fSLV3C-(IUTULSWfoIjFey8xgIxSoBo66DuNm1v0tpdsydxyK_nZW.wP*Bmfth'52(n0ToLoqndDQ0OfIzNu1YeU~hkcV9!ytM*!fd.21pQO5_GXn(z
```
*218 символов*

Base85url на 6 символов компактнее!

# Использование
```python
import b85url

text = "Этот пример текста ровно в сто символов длиной для демонстрации кодирования в base64url и base85url."

encoded_text = "CWR9X.MbxiA6W6If.~BUl7wd*pukqAlAWWy-aeOog4cLAi0)JuAzXRTDY4oyYde05abBiMfVbqDhJXqzpMuCA32l*HHcyUek0ZVDlv3fSLV3C-(IUTULSWfoIjFey8xgIxSoBo66DuNm1v0tpdsydxyK_nZW.wP*Bmfth'52(n0ToLoqndDQ0OfIzNu1YeU~hkcV9!ytM*!fd.21pQO5_GXn(z"

# Кодирование текста
print(b85url.base85url_encode(text))
# Декодирование текста
print(b85url.base85url_decode(encoded_text).decode())

# Более простые примеры

# Кодирование текста
print(b85url.encode_string(text))
# Декодирование текста
print(b85url.decode_string(encoded_text))
```
