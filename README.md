# Projeto de estrutura de um servidor web implementando normas e protocolos de segurança segundo o projeto Open Standards Everywhere

Para esse projeto foram consideradas as normas definidas pela OSE listadas abaixo:

	•IPv6
		– Nome de servidores com IPv6
		– Servidores acessíveis via IPv6
		– Servidores web com endereço IPv6
		– Servidores web acessíveis via IPv6
		– Mesmo website alcançado via IPv4 e IPv6
	
	•DNSSEC
		– Existência
		– Validação
	
	•Conexão Segura
		– HTTPS
		– Redirecionamento de HTTP para HTTPS
		– Não possuir compressão HTTP
		– Política HSTS
		– Versão de TLS atuais (1.2 ou 1.3) e versões antigas desabilitadas
		– Suporte a criptografia segura utilizando apenas cifras consideradas seguras
		– Imposição da preferência da criptografia
		– Suporte a parâmetros seguros para troca de chaves utilizando ECDHE
		– Suporte a função de hash segura para troca de chaves (SHA-256, SHA-384 ou SHA-512)
		– Não possuir compressão TLS
		– Suporte a renegociação segura
		– Bloqueio de renegociação iniciada pelo cliente
		– Não possuir suporte 0-RTT
		– Suporte ao OCSP stapling
		– Cadeia de certificado completa e assinada por uma CA
		– Certificado de chave pública com parâmetros seguros
		– Assinatura do certificado utilizando um algoritmo hash seguro
		– Nome do domínio presente no certificado
		– Existência de um registro TLSA para o DANE
		– Validação do DANE

	•Cabeçalhos HTTP
		– Utilização do CSP para proteger os visitantes de ataques como clickjacking
		– A utilização do X-Frame-Options para proteger os visitantes de navegadores mais antigos que não oferecem suporte a CSP
		– X-Content-Type-Options com valor nosniff
		– X-XSS-Protection com valor 1; mode=block para ativar a filtragem XSS. Para essa configuração o navegador impedirá a
		renderização da página se um ataque for detectado 
		– Referrer-Policy configurado com no-referrer ou same-origin quando não possui dados sensíveis para terceiros. 
		Quando possuir dados confidenciais para terceiros deve ser utilizado strict-origin ou strict-origin-when-cross-origin, apenas
		por meio de conexões seguras (HTTPS)

Dúvidas podem ser enviadas para raphaela.sgoulart@gmail.com

