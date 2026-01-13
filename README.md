
# 🎤 Assistente de Voz Multilíngue com Python, Whisper e ChatGPT

Este projeto implementa um **assistente de voz multilíngue** que combina **gravação de áudio**, **transcrição automática**, **geração de respostas inteligentes** e **síntese de voz**.  
Ele foi desenvolvido em **Python** com suporte de **JavaScript**, **Whisper (OpenAI)**, **ChatGPT** e **gTTS** com apoio da DIO e Bradesco

---

## 🚀 Funcionalidades
- 🎙️ **Gravação de áudio** diretamente no navegador via `MediaStream Recording API`.
- 🧠 **Reconhecimento de fala** com o modelo Whisper da OpenAI.
- 💬 **Integração com ChatGPT** para respostas inteligentes.
- 🔊 **Síntese de voz** com gTTS para reproduzir a resposta em áudio.
- 🌍 **Suporte multilíngue** configurável pela variável `language`.

---

## 📂 Estrutura do Projeto
1. **Gravação de Áudio (Python + JS)**  
   - Captura áudio do microfone.  
   - Converte para `.wav`.  
   - Salva no diretório `/content/` do Google Colab.  

2. **Reconhecimento de Fala (Whisper)**  
   - Instalação do Whisper via `pip`.  
   - Carregamento do modelo (`small`, mas pode ser alterado).  
   - Transcrição automática do áudio para texto.  

3. **Integração com ChatGPT**  
   - Configuração da API Key da OpenAI.  
   - Envio da transcrição para o ChatGPT.  
   - Recebimento da resposta textual.  

4. **Síntese de Voz (gTTS)**  
   - Conversão da resposta em áudio.  
   - Reprodução do áudio diretamente no Colab.  

---

## 🛠️ Requisitos
- Python 3.x  
- Google Colab (ou ambiente compatível)  
- Bibliotecas:  
  - `IPython`  
  - `google.colab`  
  - `base64`  
  - `whisper`  
  - `gtts`  

---

## 📌 Como Usar
1. Clone ou copie o código para o Google Colab.  
2. Execute as células em ordem:  
   - Gravação de áudio.  
   - Transcrição com Whisper.  
   - Integração com ChatGPT.  
   - Síntese de voz com gTTS.  
3. Configure a variável `language` para o idioma desejado (`'pt'`, `'en'`, `'es'`, etc.).  
4. Insira sua **API Key da OpenAI** em:  
   ```python
   os.environ['OPENAI_API_KEY'] = 'SUA_API_KEY_AQUI'
   ```

---

## 🌍 Idiomas Suportados
- Português (`pt`)  
- Inglês (`en`)  
- Espanhol (`es`)  
- Francês (`fr`)  
- Alemão (`de`)  
- E muitos outros suportados pelo Whisper e gTTS.  

---

## 📖 Referências
- [Whisper GitHub](https://github.com/openai/whisper)  
- [OpenAI API Documentation](https://platform.openai.com/docs/api-reference/introduction)  
- [gTTS Documentation](https://pypi.org/project/gTTS/)  
- [MediaStream Recording API](https://developer.mozilla.org/en-US/docs/Web/API/MediaStream_Recording_API)  

---

## 💡 Possíveis Melhorias
- Adicionar interface gráfica.  
- Suporte offline para síntese de voz.  
- Integração com outros modelos de IA.  
- Exportar histórico de conversas.  

---

## 📜 Licença
Este projeto é de uso livre para fins educacionais e experimentais.  

---

👉 Você gostaria que eu também criasse um **exemplo de uso passo a passo** (com código simplificado) para colocar no README, mostrando a execução completa em Colab? Isso deixaria o projeto ainda mais acessível para iniciantes.
