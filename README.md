# dio-curso-excel-claude

## 1. Perguntas que a ferramenta responde (aba Planilha1)
- Quanto devo investir por mês? → `D12` (30% do salário em `D10`) = R$ 200,00
- Quanto terei acumulado no prazo escolhido? → `D18`= 16.755,38
- Quanto isso rende de dividendos por mês? → `D19` = 100,53
- Quanto terei em 2, 5, 10, 20 e 30 anos, e com que dividendo? → `C22:D26` =
Patrimônio acumulado respectivamente:
R$ 5.445,53
R$ 16.755,38
R$ 48.656,84
R$ 225.039,68
R$ 864.433,93
Dividento respectivamente:
R$ 32,67
R$ 100,53
R$ 291,94
R$ 1.350,24
R$ 5.186,60

CONFIGURAÇÕES		
Salário		R$ 2.000,00
Rendimento Carteria		0,60%
Sugestão investimento		R$ 600,00
		
INVESTIMENTO MENSAL		
Quanto investir mês		R$ 200,00
Quantos anos		5
Taxa de rendimento mensal		1,079%
Patrimônio Acumulado		R$ 16.755,38
Dividendos Mensais		R$ 100,53
		
Cenários		Dividendo
Quanto em 2 anos 	R$ 5.445,53	R$ 32,67
Quanto em 5 anos	R$ 16.755,38	R$ 100,53
Quanto em 10 anos	R$ 48.656,84	R$ 291,94
Quanto em 20 anos	R$ 225.039,68	R$ 1.350,24
Quanto em 30 anos	R$ 864.433,93	R$ 5.186,60
<img width="649" height="403" alt="image" src="https://github.com/user-attachments/assets/c6bf4339-da0e-4993-8f6c-7c3d4e019fb2" />



- Como dividir o aporte entre os tipos de FII, de acordo com o meu perfil? → Alterando a lista suspensa em C30 (percentuais em `C34:C39`, valores em `D34:D39`, total em `D40` e gráfico de pizza a partir de `B42`)
  CONSERVADOR
 Perfil	CONSERVADOR	
Valor a ser investido mês	R$ 200,00	
		
TIPOS DE FIIS	Percentual Sugerido	Valores
PAPEL	30%	R$ 60,00
TIJOLO	50%	R$ 100,00
HÍBRIDOS	10%	R$ 20,00
FOF´S	10%	R$ 20,00
DESENVOLVIMENTO	0%	R$ 0,00
HOTELARIAS	0%	R$ 0,00
		R$ 200,00
<img width="649" height="198" alt="image" src="https://github.com/user-attachments/assets/fe329e02-2787-4d29-9361-fff4d81d6f27" />


Perfil	MODERADO	
Valor a ser investido mês	R$ 200,00	
		
TIPOS DE FIIS	Percentual Sugerido	Valores
PAPEL	32%	R$ 64,00
TIJOLO	35%	R$ 70,00
HÍBRIDOS	8%	R$ 16,00
FOF´S	5%	R$ 10,00
DESENVOLVIMENTO	10%	R$ 20,00
HOTELARIAS	10%	R$ 20,00
		R$ 200,00
<img width="649" height="198" alt="image" src="https://github.com/user-attachments/assets/a2a2d2a8-659d-4028-b558-24b669e01e84" />

Perfil	AGRESSIVO	
Valor a ser investido mês	R$ 200,00	
		
TIPOS DE FIIS	Percentual Sugerido	Valores
PAPEL	50%	R$ 100,00
TIJOLO	10%	R$ 20,00
HÍBRIDOS	5%	R$ 10,00
FOF´S	5%	R$ 10,00
DESENVOLVIMENTO	20%	R$ 40,00
HOTELARIAS	10%	R$ 20,00
		R$ 200,00
<img width="649" height="198" alt="image" src="https://github.com/user-attachments/assets/b10fc1e1-3a1f-47d7-af26-3b4a7c163244" />



## 2. Como o VF e o PROCV entram
- **VF** calcula o patrimônio futuro com aportes mensais: `=VF(taxa mensal; anos*12; -aporte)`. É usado em `D18` e em `C22:C26`.
- **PROCV** busca o percentual de cada tipo de FII. A fórmula junta perfil e tipo (ex.: `MODERADO-PAPEL`) e procura essa chave na Planilha2: `=PROCV($C$30&"-"&B34;Planilha2!$A:$D;4;FALSO)`. Ao trocar o perfil em `C30`, os percentuais, os valores e o gráfico são atualizados.

## 3. Intervalos nomeados
`salario` (D10), `Rendimento_carteira` (D11), `sugestao_investimento` (D12), `Aporte` (D15), `qtd_anos` (D16), `taxa_mensal` (D17) e `patrimonio` (D18).

## 4. Percentuais de cada perfil (Planilha2)

| Tipo | Conservador | Moderado | Agressivo |
|---|---|---|---|
| Papel           | 30% | 32% | 50% |
| Tijolo          | 50% | 35% | 10% |
| Híbridos        | 10% | 8% | 5% |
| FOFs            | 10% | 5% | 5% |
| Desenvolvimento | 0% | 10% | 20% |
| Hotelarias      | 0% | 10% | 10% |



## 5. O que mudou em relação à ferramenta do Expert
Deixei a legenda no gráfico de "pizza" e alguns detalhes de formatação

<img width="530" height="283" alt="image" src="https://github.com/user-attachments/assets/56a261cc-a76e-478a-8901-b64511fb358b" />

<img width="530" height="283" alt="image" src="https://github.com/user-attachments/assets/f6bc81a7-870b-49f7-810a-a3ef139892ed" />

<img width="530" height="283" alt="image" src="https://github.com/user-attachments/assets/9aa1f43e-efee-4fc9-baf3-1d39ef3fe115" />





