# Arquitetura Hexagonal - Ports and Adpapters
## Introdução

<img src="/assets/images/port-and-adapters.png" style="height: 300px; width:400px;"/>

"Allow an application to equally be driven by users, programs, automated test or batch scripts, and to be developed and tested in isolation from its eventual run-time devices and datavases." - Cockburn

<b>Opnião Wesley willians:</b> O termo "Arquitetura" Hexagonal está muito mais ligado com decisões de design de software do que necessariamente de arquitetura.

### Pontos importantes sobre arquitetura
- **Crescimento sustentável:** conforme você desenvolve um software ao longo do tempo e mantém ele sem débito técnico e sem retrabalho;
- **Software precisa se pagar ao passar do tempo:** a empresa precisa receber retorno do software desenvolvido;
- **Software deve ser desenhado por você e não pelo seu framework:** a complexidade do problema do negócio não pode estar atrelada a complexidade técnica do framework;
- **Peças precisam se encaixar e eventualmente substituídas:** tem que ser possível substituir as peças utilizada para desenvolver o sistema.

**Arquitetura diz respeito com o futuro do seu software. CRUD qualquer um faz!**

### Ciclo de vida de muitos projetos
**Fase 1, 2, 3:**

<img src="/assets/images/fase-1-2-3.png" style="height: 300px; width:400px;"/>

**Fase 4, 5, 6:**

<img src="/assets/images/fase-4-5-6.png" style="height: 300px; width:400px;"/>

**Fase 7, 8, 9:**

<img src="/assets/images/fase-7-8-9.png" style="height: 300px; width:400px;"/>

**Fase 10:**

<img src="/assets/images/fase-10.png" style="height: 200px; width:200px;"/>

#### Principais problemas encontrados nas fases do projeto
- Faltou <b>visão do futuro</b>. Devemos sempre considerar que o sistema vai crescer;
- <b>Limites bem definidos</b>. Limites bem definidos consegue manter o negócio não misturado com o framework;
- <b>Troca e adição de componentes</b>. Se você não consegue trocar um componente por outro, quer dizer que seu sistema está com alto acoplamento;
- <b>Escala</b>. O processo de escala sempre vai dar problema se não tivermos visão de futuro. A visão de possuir escala <b>horizontal</b> tem que estar presente desde o dia número 1;
- <b>Otimizações frequentes</b> o desenvolvilmento focado apenas em features sempre acaba deixando alguns débitos técnicos para trás. O grande ponto é que com limites nós conseguimos impedir que um débito técnico se junte com outro débito técnico;
- <b>Preparado para mudanças</b>. Conseguimos efetuar mudanças bruscas no sistema, troca de CRM, de Gateway de pagamento, etc.

#### Reflexões encontradas
- Está sendo doloroso para o desenvolvedor atualiza o software?
- Os problemas poderiam ter sido evitados?
- Todo o investimento teve retorno? O software está se pagando?
- Será que a relação com o cliente está boa?
- Será que o cliente terá prejuízo com a brusca mudança arquitetural?
- Em qual momento tudo se perdeu?
    - Ele começou a se perder a partir do dia 1.
- Se você fosse novo na equipe, você julgaria os devs que fizeram tudo isso?
