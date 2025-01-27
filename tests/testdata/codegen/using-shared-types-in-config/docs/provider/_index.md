
---
title: "Provider"
title_tag: "credentials.Provider"
meta_desc: "Documentation for the credentials.Provider resource with examples, input properties, output properties, lookup functions, and supporting types."
layout: api
no_edit_this_page: true
---



<!-- WARNING: this file was generated by test. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->




## Create Provider Resource {#create}

Resources are created with functions called constructors. To learn more about declaring and configuring resources, see [Resources](/docs/concepts/resources/).

### Constructor syntax
<div>
<pulumi-chooser type="language" options="typescript,python,go,csharp,java,yaml"></pulumi-chooser>
</div>


<div>
<pulumi-choosable type="language" values="javascript,typescript">
<div class="no-copy"><div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx">Provider</span><span class="p">(</span><span class="nx">name</span><span class="p">:</span> <span class="nx">string</span><span class="p">,</span> <span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="#inputs">ProviderArgs</a></span><span class="p">,</span> <span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
</div></pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="python">
<div class="no-copy"><div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class=nd>@overload</span>
<span class="k">def </span><span class="nx">Provider</span><span class="p">(</span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">str</span><span class="p">,</span>
             <span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="#inputs">ProviderArgs</a></span><span class="p">,</span>
             <span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">Optional[ResourceOptions]</a></span> = None<span class="p">)</span>
<span></span>
<span class=nd>@overload</span>
<span class="k">def </span><span class="nx">Provider</span><span class="p">(</span><span class="nx">resource_name</span><span class="p">:</span> <span class="nx">str</span><span class="p">,</span>
             <span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">Optional[ResourceOptions]</a></span> = None<span class="p">,</span>
             <span class="nx">hash</span><span class="p">:</span> <span class="nx">Optional[HashKind]</span> = None<span class="p">,</span>
             <span class="nx">password</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">,</span>
             <span class="nx">shared</span><span class="p">:</span> <span class="nx">Optional[SharedArgs]</span> = None<span class="p">,</span>
             <span class="nx">user</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">)</span></code></pre></div>
</div></pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="go">
<div class="no-copy"><div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span><span class="nx">NewProvider</span><span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v3/go/pulumi?tab=doc#Context">Context</a></span><span class="p">,</span> <span class="nx">name</span><span class="p"> </span><span class="nx">string</span><span class="p">,</span> <span class="nx">args</span><span class="p"> </span><span class="nx"><a href="#inputs">ProviderArgs</a></span><span class="p">,</span> <span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v3/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx">Provider</span>, error)</span></code></pre></div>
</div></pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="csharp">
<div class="no-copy"><div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx">Provider</span><span class="p">(</span><span class="nx">string</span><span class="p"> </span><span class="nx">name<span class="p">,</span> <span class="nx"><a href="#inputs">ProviderArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">,</span> <span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span></code></pre></div>
</div></pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="java">
<div class="no-copy"><div class="highlight"><pre class="chroma">
<code class="language-java" data-lang="java"><span class="k">public </span><span class="nx">Provider</span><span class="p">(</span><span class="nx">String</span><span class="p"> </span><span class="nx">name<span class="p">,</span> <span class="nx"><a href="#inputs">ProviderArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">)</span>
<span class="k">public </span><span class="nx">Provider</span><span class="p">(</span><span class="nx">String</span><span class="p"> </span><span class="nx">name<span class="p">,</span> <span class="nx"><a href="#inputs">ProviderArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">,</span> <span class="nx">CustomResourceOptions</span><span class="p"> </span><span class="nx">options<span class="p">)</span>
</code></pre></div></div>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="yaml">
<div class="no-copy"><div class="highlight"><pre class="chroma"><code class="language-yaml" data-lang="yaml">type: <span class="nx">pulumi:providers:credentials</span><span class="p"></span>
<span class="p">properties</span><span class="p">: </span><span class="c">#&nbsp;The arguments to resource properties.</span>
<span class="p"></span><span class="p">options</span><span class="p">: </span><span class="c">#&nbsp;Bag of options to control resource&#39;s behavior.</span>
<span class="p"></span>
</code></pre></div></div>
</pulumi-choosable>
</div>

#### Parameters

<div>
<pulumi-choosable type="language" values="javascript,typescript">

<dl class="resources-properties"><dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>The unique name of the resource.</dd><dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">ProviderArgs</a></span>
    </dt>
    <dd>The arguments to resource properties.</dd><dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span>
    </dt>
    <dd>Bag of options to control resource&#39;s behavior.</dd></dl>

</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="python">

<dl class="resources-properties"><dt
        class="property-required" title="Required">
        <span>resource_name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>The unique name of the resource.</dd><dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">ProviderArgs</a></span>
    </dt>
    <dd>The arguments to resource properties.</dd><dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/python/pulumi/#pulumi.ResourceOptions">ResourceOptions</a></span>
    </dt>
    <dd>Bag of options to control resource&#39;s behavior.</dd></dl>

</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="go">

<dl class="resources-properties"><dt
        class="property-optional" title="Optional">
        <span>ctx</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v3/go/pulumi?tab=doc#Context">Context</a></span>
    </dt>
    <dd>Context object for the current deployment.</dd><dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>The unique name of the resource.</dd><dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">ProviderArgs</a></span>
    </dt>
    <dd>The arguments to resource properties.</dd><dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v3/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span>
    </dt>
    <dd>Bag of options to control resource&#39;s behavior.</dd></dl>

</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="csharp">

<dl class="resources-properties"><dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>The unique name of the resource.</dd><dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">ProviderArgs</a></span>
    </dt>
    <dd>The arguments to resource properties.</dd><dt
        class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>
    </dt>
    <dd>Bag of options to control resource&#39;s behavior.</dd></dl>

</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="java">

<dl class="resources-properties"><dt
        class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">String</span>
    </dt>
    <dd>The unique name of the resource.</dd><dt
        class="property-required" title="Required">
        <span>args</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#inputs">ProviderArgs</a></span>
    </dt>
    <dd>The arguments to resource properties.</dd><dt
        class="property-optional" title="Optional">
        <span>options</span>
        <span class="property-indicator"></span>
        <span class="property-type">CustomResourceOptions</span>
    </dt>
    <dd>Bag of options to control resource&#39;s behavior.</dd></dl>

</pulumi-choosable>
</div>



## Provider Resource Properties {#properties}

To learn more about resource properties and how to use them, see [Inputs and Outputs](/docs/intro/concepts/inputs-outputs) in the Architecture and Concepts docs.

### Inputs

The Provider resource accepts the following [input](/docs/intro/concepts/inputs-outputs) properties:



<div>
<pulumi-choosable type="language" values="csharp">
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="hash_csharp">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#hash_csharp" style="color: inherit; text-decoration: inherit;">Hash</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#hashkind">Pulumi.<wbr>Credentials.<wbr>Hash<wbr>Kind</a></span>
    </dt>
    <dd>The (entirely uncryptographic) hash function used to encode the &quot;password&quot;.</dd><dt class="property-required"
            title="Required">
        <span id="shared_csharp">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#shared_csharp" style="color: inherit; text-decoration: inherit;">Shared</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#shared">Shared</a></span>
    </dt>
    <dd></dd><dt class="property-required"
            title="Required">
        <span id="user_csharp">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#user_csharp" style="color: inherit; text-decoration: inherit;">User</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>The username. Its important but not secret.</dd><dt class="property-optional"
            title="Optional">
        <span id="password_csharp">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#password_csharp" style="color: inherit; text-decoration: inherit;">Password</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>The password. It is very secret. It can also be sourced from the following environment variable: <code>FOO</code></dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="go">
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="hash_go">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#hash_go" style="color: inherit; text-decoration: inherit;">Hash</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#hashkind">Hash<wbr>Kind</a></span>
    </dt>
    <dd>The (entirely uncryptographic) hash function used to encode the &quot;password&quot;.</dd><dt class="property-required"
            title="Required">
        <span id="shared_go">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#shared_go" style="color: inherit; text-decoration: inherit;">Shared</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#shared">Shared<wbr>Args</a></span>
    </dt>
    <dd></dd><dt class="property-required"
            title="Required">
        <span id="user_go">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#user_go" style="color: inherit; text-decoration: inherit;">User</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>The username. Its important but not secret.</dd><dt class="property-optional"
            title="Optional">
        <span id="password_go">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#password_go" style="color: inherit; text-decoration: inherit;">Password</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>The password. It is very secret. It can also be sourced from the following environment variable: <code>FOO</code></dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="java">
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="hash_java">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#hash_java" style="color: inherit; text-decoration: inherit;">hash</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#hashkind">Hash<wbr>Kind</a></span>
    </dt>
    <dd>The (entirely uncryptographic) hash function used to encode the &quot;password&quot;.</dd><dt class="property-required"
            title="Required">
        <span id="shared_java">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#shared_java" style="color: inherit; text-decoration: inherit;">shared</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#shared">Shared</a></span>
    </dt>
    <dd></dd><dt class="property-required"
            title="Required">
        <span id="user_java">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#user_java" style="color: inherit; text-decoration: inherit;">user</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">String</span>
    </dt>
    <dd>The username. Its important but not secret.</dd><dt class="property-optional"
            title="Optional">
        <span id="password_java">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#password_java" style="color: inherit; text-decoration: inherit;">password</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">String</span>
    </dt>
    <dd>The password. It is very secret. It can also be sourced from the following environment variable: <code>FOO</code></dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="javascript,typescript">
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="hash_nodejs">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#hash_nodejs" style="color: inherit; text-decoration: inherit;">hash</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#hashkind">Hash<wbr>Kind</a></span>
    </dt>
    <dd>The (entirely uncryptographic) hash function used to encode the &quot;password&quot;.</dd><dt class="property-required"
            title="Required">
        <span id="shared_nodejs">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#shared_nodejs" style="color: inherit; text-decoration: inherit;">shared</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#shared">Shared</a></span>
    </dt>
    <dd></dd><dt class="property-required"
            title="Required">
        <span id="user_nodejs">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#user_nodejs" style="color: inherit; text-decoration: inherit;">user</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>The username. Its important but not secret.</dd><dt class="property-optional"
            title="Optional">
        <span id="password_nodejs">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#password_nodejs" style="color: inherit; text-decoration: inherit;">password</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>The password. It is very secret. It can also be sourced from the following environment variable: <code>FOO</code></dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="python">
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="hash_python">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#hash_python" style="color: inherit; text-decoration: inherit;">hash</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#hashkind">Hash<wbr>Kind</a></span>
    </dt>
    <dd>The (entirely uncryptographic) hash function used to encode the &quot;password&quot;.</dd><dt class="property-required"
            title="Required">
        <span id="shared_python">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#shared_python" style="color: inherit; text-decoration: inherit;">shared</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#shared">Shared<wbr>Args</a></span>
    </dt>
    <dd></dd><dt class="property-required"
            title="Required">
        <span id="user_python">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#user_python" style="color: inherit; text-decoration: inherit;">user</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>The username. Its important but not secret.</dd><dt class="property-optional"
            title="Optional">
        <span id="password_python">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#password_python" style="color: inherit; text-decoration: inherit;">password</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>The password. It is very secret. It can also be sourced from the following environment variable: <code>FOO</code></dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="yaml">
<dl class="resources-properties"><dt class="property-required"
            title="Required">
        <span id="hash_yaml">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#hash_yaml" style="color: inherit; text-decoration: inherit;">hash</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#hashkind">&#34;Adler32&#34; | &#34;CRC32&#34;</a></span>
    </dt>
    <dd>The (entirely uncryptographic) hash function used to encode the &quot;password&quot;.</dd><dt class="property-required"
            title="Required">
        <span id="shared_yaml">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#shared_yaml" style="color: inherit; text-decoration: inherit;">shared</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#shared">Property Map</a></span>
    </dt>
    <dd></dd><dt class="property-required"
            title="Required">
        <span id="user_yaml">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#user_yaml" style="color: inherit; text-decoration: inherit;">user</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">String</span>
    </dt>
    <dd>The username. Its important but not secret.</dd><dt class="property-optional"
            title="Optional">
        <span id="password_yaml">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#password_yaml" style="color: inherit; text-decoration: inherit;">password</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">String</span>
    </dt>
    <dd>The password. It is very secret. It can also be sourced from the following environment variable: <code>FOO</code></dd></dl>
</pulumi-choosable>
</div>


### Outputs

All [input](#inputs) properties are implicitly available as output properties. Additionally, the Provider resource produces the following output properties:



<div>
<pulumi-choosable type="language" values="csharp">
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="id_csharp">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>The provider-assigned unique ID for this managed resource.</dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="go">
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="id_go">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>The provider-assigned unique ID for this managed resource.</dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="java">
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="id_java">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#id_java" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">String</span>
    </dt>
    <dd>The provider-assigned unique ID for this managed resource.</dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="javascript,typescript">
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="id_nodejs">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>The provider-assigned unique ID for this managed resource.</dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="python">
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="id_python">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>The provider-assigned unique ID for this managed resource.</dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="yaml">
<dl class="resources-properties"><dt class="property-"
            title="">
        <span id="id_yaml">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#id_yaml" style="color: inherit; text-decoration: inherit;">id</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">String</span>
    </dt>
    <dd>The provider-assigned unique ID for this managed resource.</dd></dl>
</pulumi-choosable>
</div>







## Supporting Types



<h4 id="hashkind">
Hash<wbr>Kind<pulumi-choosable type="language" values="python,go" class="inline">, Hash<wbr>Kind<wbr>Args</pulumi-choosable>
</h4>

<div>
<pulumi-choosable type="language" values="csharp">
<dl class="tabular"><dt>Adler32</dt>
    <dd>Adler32Adler32 implements the Adler-32 checksum.</dd><dt>CRC32</dt>
    <dd>CRC32CRC32 implements the 32-bit cyclic redundancy check, or CRC-32, checksum.</dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="go">
<dl class="tabular"><dt>Hash<wbr>Kind<wbr>Adler32</dt>
    <dd>Adler32Adler32 implements the Adler-32 checksum.</dd><dt>Hash<wbr>Kind<wbr>CRC32</dt>
    <dd>CRC32CRC32 implements the 32-bit cyclic redundancy check, or CRC-32, checksum.</dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="java">
<dl class="tabular"><dt>Adler32</dt>
    <dd>Adler32Adler32 implements the Adler-32 checksum.</dd><dt>CRC32</dt>
    <dd>CRC32CRC32 implements the 32-bit cyclic redundancy check, or CRC-32, checksum.</dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="javascript,typescript">
<dl class="tabular"><dt>Adler32</dt>
    <dd>Adler32Adler32 implements the Adler-32 checksum.</dd><dt>CRC32</dt>
    <dd>CRC32CRC32 implements the 32-bit cyclic redundancy check, or CRC-32, checksum.</dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="python">
<dl class="tabular"><dt>ADLER32</dt>
    <dd>Adler32Adler32 implements the Adler-32 checksum.</dd><dt>CRC32</dt>
    <dd>CRC32CRC32 implements the 32-bit cyclic redundancy check, or CRC-32, checksum.</dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="yaml">
<dl class="tabular"><dt>"Adler32"</dt>
    <dd>Adler32Adler32 implements the Adler-32 checksum.</dd><dt>"CRC32"</dt>
    <dd>CRC32CRC32 implements the 32-bit cyclic redundancy check, or CRC-32, checksum.</dd></dl>
</pulumi-choosable>
</div>

<h4 id="shared">
Shared<pulumi-choosable type="language" values="python,go" class="inline">, Shared<wbr>Args</pulumi-choosable>
</h4>

<div>
<pulumi-choosable type="language" values="csharp">
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="foo_csharp">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#foo_csharp" style="color: inherit; text-decoration: inherit;">Foo</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd></dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="go">
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="foo_go">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#foo_go" style="color: inherit; text-decoration: inherit;">Foo</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd></dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="java">
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="foo_java">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#foo_java" style="color: inherit; text-decoration: inherit;">foo</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">String</span>
    </dt>
    <dd></dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="javascript,typescript">
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="foo_nodejs">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#foo_nodejs" style="color: inherit; text-decoration: inherit;">foo</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd></dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="python">
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="foo_python">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#foo_python" style="color: inherit; text-decoration: inherit;">foo</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd></dd></dl>
</pulumi-choosable>
</div>

<div>
<pulumi-choosable type="language" values="yaml">
<dl class="resources-properties"><dt class="property-optional"
            title="Optional">
        <span id="foo_yaml">
<a data-swiftype-name="resource-property" data-swiftype-type="text" href="#foo_yaml" style="color: inherit; text-decoration: inherit;">foo</a>
</span>
        <span class="property-indicator"></span>
        <span class="property-type">String</span>
    </dt>
    <dd></dd></dl>
</pulumi-choosable>
</div>


<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="">credentials </a></dd>
	<dt>License</dt>
	<dd></dd>
</dl>

