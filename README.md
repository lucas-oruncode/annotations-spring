# Anotações Principais do Spring Framework

Este documento descreve as principais anotações utilizadas no **Spring Framework** e suas funcionalidades, organizadas por categorias.

---

## 1. **Anotações de Configuração**

- **`@Configuration`**  
  Marca uma classe como fonte de definições de beans.

- **`@Bean`**  
  Indica que o método produzirá um bean a ser gerenciado pelo contêiner Spring.

- **`@ComponentScan`**  
  Configura o escaneamento de pacotes para encontrar componentes, serviços e repositórios.

- **`@PropertySource`**  
  Carrega arquivos de propriedades externos no ambiente Spring.

---

## 2. **Anotações de Componente**

- **`@Component`**  
  Marca uma classe como um componente genérico gerenciado pelo contêiner Spring.

- **`@Service`**  
  Específica para classes de serviço. É semanticamente equivalente a `@Component`.

- **`@Repository`**  
  Usada para classes de acesso a dados (DAO). Também fornece tratamento especial para exceções relacionadas ao banco de dados.

- **`@Controller`**  
  Marca uma classe como controlador em aplicações Spring MVC.

---

## 3. **Injeção de Dependência**

- **`@Autowired`**  
  Injeta automaticamente uma dependência pelo tipo.

- **`@Qualifier`**  
  Usada em conjunto com `@Autowired` para especificar o bean exato a ser injetado.

- **`@Value`**  
  Injeta valores de propriedades no bean.

---

## 4. **Spring Boot**

- **`@SpringBootApplication`**  
  Combina as anotações `@Configuration`, `@EnableAutoConfiguration` e `@ComponentScan`.

- **`@EnableAutoConfiguration`**  
  Permite a configuração automática baseada nas dependências do classpath.

- **`@RestController`**  
  Combina `@Controller` e `@ResponseBody` para simplificar controladores RESTful.

---

## 5. **Anotações de Web (Spring MVC)**

- **`@RequestMapping`**  
  Define o mapeamento de URLs para métodos ou classes.

- **`@GetMapping`**, **`@PostMapping`**, **`@PutMapping`**, **`@DeleteMapping`**, **`@PatchMapping`**  
  Anotações específicas para mapeamento de métodos HTTP.

- **`@PathVariable`**  
  Injeta valores de variáveis de caminho em um método.

- **`@RequestParam`**  
  Injeta parâmetros de consulta (query parameters) no método.

- **`@RequestBody`**  
  Converte o corpo de uma requisição JSON em um objeto Java.

- **`@ResponseBody`**  
  Converte o retorno de um método em JSON ou XML para a resposta HTTP.

---

## 6. **Anotações de Banco de Dados (Spring Data)**

- **`@Entity`**  
  Marca uma classe como uma entidade JPA.

- **`@Id`**  
  Define o identificador único de uma entidade.

- **`@GeneratedValue`**  
  Especifica como o valor do identificador será gerado.

- **`@Table`**  
  Define detalhes sobre a tabela associada a uma entidade.

- **`@Transactional`**  
  Garante que métodos ou classes sejam executados em transações.

---

## 7. **Anotações de Controle de Transação**

- **`@EnableTransactionManagement`**  
  Habilita o gerenciamento de transações no Spring.

- **`@Transactional`**  
  Gerencia transações para métodos ou classes, garantindo consistência.

---

## 8. **Anotações de Teste**

- **`@SpringBootTest`**  
  Carrega o contexto completo da aplicação para testes de integração.

- **`@MockBean`**  
  Cria e injeta um mock (falso) de um bean no contexto.

- **`@WebMvcTest`**  
  Carrega apenas componentes Spring MVC, como controladores.

- **`@DataJpaTest`**  
  Configura o contexto para testes com Spring Data JPA.

---

Essas anotações cobrem os cenários mais comuns no desenvolvimento de aplicações Spring. 
