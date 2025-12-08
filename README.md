- 👋 Hi, I’m Pedro Marsão
- 👀 I’m interested in java e kotlin programer
- 🌱 I’m currently learning React
<!---
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
-->
## 🛠️ My desktop setup:

1. Oh My Zsh is a delightful, open source, community-driven framework for managing your Zsh configuration. It comes bundled with thousands of helpful functions, helpers, plugins, themes, and a few things that make you shout... [Oh My Zsh](https://ohmyz.sh/)

    * Plugins 
        - git
        - bgnotify
        - command-not-found
        - zsh-autosuggestions `git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`
        - zsh-peco-history `git clone https://github.com/jimeh/zsh-peco-history.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-peco-history`
        - sudo
2. Meet SDKMAN! – your reliable companion for effortlessly managing multiple Software Development Kits on Unix systems. Imagine having different versions of SDKs and needing a stress-free way to switch between them. SDKMAN! steps in with its easy-to-use Command Line Interface (CLI) and API. Formerly known as GVM, the Groovy enVironment Manager, SDKMAN! draws inspiration from familiar tools like apt, pip, RVM, and rbenv and even Git. Think of it as your helpful toolkit friend, ready to streamline SDK management for you [SDKMAN!](https://sdkman.io/)
3. Guake Terminal is a simple and practical way to quickly access your terminal in Gnome, to run your commands. [Guake Terminal](https://guake.github.io/)

4. IntelliJ IDEA Community Edition - [Intellij](https://download.jetbrains.com/idea/ideaIC-2025.2.5-aarch64.tar.gz?_gl=1*12d1z4v*_gcl_au*MTg3NDk0MDE1NC4xNzY0MDI2MzAy*FPAU*MTg3NDk0MDE1NC4xNzY0MDI2MzAy*_ga*OTU4OTk3NzE2LjE3NjQwMjYzMDI.*_ga_9J976DJZ68*czE3NjQ5NjE2NDgkbzUkZzEkdDE3NjQ5NjE3NTIkajQ0JGwwJGgw)

5. My Intellij Code Style
```
<?xml version="1.0" encoding="UTF-8"?>
<code_scheme name="BackendPedroStyle" version="173">

  <!-- ===== Geral ===== -->
  <!-- Boa largura pra backend (logs, builders etc.) -->
  <option name="RIGHT_MARGIN" value="120"/>

  <!-- ==================== JAVA ==================== -->
  <JavaCodeStyleSettings>
    <!-- Nunca usar import com '*' -->
    <option name="CLASS_COUNT_TO_USE_IMPORT_ON_DEMAND" value="9999"/>
    <option name="NAMES_COUNT_TO_USE_IMPORT_ON_DEMAND" value="9999"/>

    <!-- Não usar import-on-demand em nenhum pacote -->
    <option name="PACKAGES_TO_USE_IMPORT_ON_DEMAND">
      <value/>
    </option>

    <!-- Layout de imports: mais usados em backend primeiro -->
    <option name="IMPORT_LAYOUT_TABLE">
      <value>
        <!-- Core Java -->
        <package name="java" withSubpackages="true" static="false"/>
        <emptyLine/>
        <package name="javax" withSubpackages="true" static="false"/>
        <emptyLine/>
        <package name="jakarta" withSubpackages="true" static="false"/>
        <emptyLine/>

        <!-- Spring e libs de backend comuns -->
        <package name="org.springframework" withSubpackages="true" static="false"/>
        <emptyLine/>
        <package name="org" withSubpackages="true" static="false"/>
        <emptyLine/>
        <package name="com" withSubpackages="true" static="false"/>
        <emptyLine/>

        <!-- Qualquer outro -->
        <package name="" withSubpackages="true" static="false"/>
        <emptyLine/>

        <!-- Imports estáticos por último -->
        <package name="" withSubpackages="true" static="true"/>
      </value>
    </option>

    <!-- Útil em backend pra imutabilidade local -->
    <option name="GENERATE_FINAL_LOCALS" value="true"/>
    <option name="GENERATE_FINAL_PARAMETERS" value="true"/>
  </JavaCodeStyleSettings>

  <codeStyleSettings language="JAVA">
    <!-- Deixar o código “respirar”, mas sem virar um queijo suíço -->
    <option name="KEEP_BLANK_LINES_IN_DECLARATIONS" value="1"/>
    <option name="KEEP_BLANK_LINES_IN_CODE" value="1"/>
    <option name="KEEP_BLANK_LINES_BEFORE_RBRACE" value="0"/>

    <!-- Quebras de linha para legibilidade de métodos e chamadas  -->
    <option name="CALL_PARAMETERS_WRAP" value="1"/>           <!-- WRAP_AS_NEEDED -->
    <option name="METHOD_PARAMETERS_WRAP" value="1"/>         <!-- WRAP_AS_NEEDED -->
    <option name="RESOURCE_LIST_WRAP" value="1"/>
    <option name="BINARY_OPERATION_WRAP" value="1"/>
    <option name="BINARY_OPERATION_SIGN_ON_NEXT_LINE" value="true"/>
    <option name="TERNARY_OPERATION_WRAP" value="1"/>
    <option name="TERNARY_OPERATION_SIGNS_ON_NEXT_LINE" value="true"/>
    <option name="FOR_STATEMENT_WRAP" value="1"/>
    <option name="ARRAY_INITIALIZER_WRAP" value="1"/>
    <option name="ASSIGNMENT_WRAP" value="1"/>
    <option name="WRAP_LONG_LINES" value="true"/>

    <!-- Backend normalmente prefere sempre chaves -->
    <option name="IF_BRACE_FORCE" value="1"/>       <!-- FORCE_BRACES_IF_MULTILINE / ALWAYS -->
    <option name="WHILE_BRACE_FORCE" value="1"/>
    <option name="FOR_BRACE_FORCE" value="1"/>
    <option name="DOWHILE_BRACE_FORCE" value="1"/>

    <!-- Métodos mais claros (não tudo em uma linha) -->
    <option name="KEEP_SIMPLE_METHODS_IN_ONE_LINE" value="false"/>

    <!-- Indentação -->
    <indentOptions>
      <option name="INDENT_SIZE" value="4"/>
      <option name="CONTINUATION_INDENT_SIZE" value="8"/>
      <option name="TAB_SIZE" value="4"/>
      <option name="USE_TAB_CHARACTER" value="false"/>
    </indentOptions>
  </codeStyleSettings>

  <!-- ==================== KOTLIN ==================== -->
  <KotlinCodeStyleSettings>
    <!-- Nada de star import em Kotlin também -->
    <option name="NAME_COUNT_TO_USE_STAR_IMPORT" value="9999"/>
    <option name="NAME_COUNT_TO_USE_STAR_IMPORT_FOR_MEMBERS" value="9999"/>

    <!-- Não usar star-import nem pra determinados pacotes -->
    <option name="PACKAGES_TO_USE_STAR_IMPORTS">
      <value/>
    </option>

    <!-- Mantém estilo mais legível para backend (padrão "IntelliJ" ajustado) -->
    <option name="CODE_STYLE_DEFAULTS" value="KOTLIN_OFFICIAL"/>
  </KotlinCodeStyleSettings>

  <codeStyleSettings language="kotlin">
    <!-- Espaços em branco parecidos com Java -->
    <option name="KEEP_BLANK_LINES_IN_DECLARATIONS" value="1"/>
    <option name="KEEP_BLANK_LINES_IN_CODE" value="1"/>
    <option name="KEEP_BLANK_LINES_BEFORE_RBRACE" value="0"/>

    <!-- Quebra de linha em parâmetros de funções maiores -->
    <option name="CALL_PARAMETERS_WRAP" value="1"/>
    <option name="METHOD_PARAMETERS_WRAP" value="1"/>
    <option name="WRAP_LONG_LINES" value="true"/>

    <!-- Indentação Kotlin: 4 espaços -->
    <indentOptions>
      <option name="INDENT_SIZE" value="4"/>
      <option name="CONTINUATION_INDENT_SIZE" value="8"/>
      <option name="TAB_SIZE" value="4"/>
      <option name="USE_TAB_CHARACTER" value="false"/>
    </indentOptions>
  </codeStyleSettings>

</code_scheme>

```


<!---
pemarsao/pemarsao is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
