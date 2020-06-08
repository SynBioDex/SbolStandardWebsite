---
id: 1874
title: SBOL 2.1.0 Released
date: 2017-01-16T06:33:46+00:00
author: Tramy Nguyen
layout: post
guid: http://sbolstandard.org/?p=1874
permalink: /sbol-2-1-0-released/
categories:
  - Announcements
---
<p class="p1">
  <span class="s1">SBOL version 2.1 has now been officially released. This is a backwards-compatible release extending the data model and updating ontology terms and best practices. In addition to minor textual updates and corrections, the key changes are:</span>
</p>

<ul class="ul1">
  <li class="li1">
    <span class="s1">&#8220;role&#8221; is added to Component and SequenceAnnotation, &#8220;roleIntegration&#8221; allows a Component role to override a ComponentDefinition role in context. SequenceAnnotation roles are used for marking features that should not have their own ComponentDefinition (e.g., restriction sites, imported GenBank features)</span>
  </li>
  <li class="li1">
    <span class="s1">SBO terms added to fill out recommended Interaction and Participation tables</span>
  </li>
  <li class="li1">
    <span class="s1">Best practices for representing topology (e.g., circular vs. linear DNA) using SequenceOntology types</span>
  </li>
  <li class="li1">
    <span class="s1">Best practices for tracking provenance</span>
  </li>
  <li class="li1">
    <span class="s1">Best practices for dealing with RDF compliance issues on <a href="http://identifiers.org/"><span class="s3">identifiers.org</span></a> by alternative use of equivalent compliant <a href="http://purl.org/"><span class="s3">purl.org</span></a> URIs</span>
  </li>
  <li class="li1">
    <span class="s1">Differences from v2.0 are marked by colored text and change-bars.</span>
  </li>
</ul>

<p class="p1">
  <span class="s1">The official release is also <a href="https://github.com/SynBioDex/SBOL-specification/releases/download/v2.1.0/BBF-RFC112-SBOL2.1.0.pdf"><span class="s3">available on GitHub</span></a> and the <a href="http://sbolstandard.org">SBOL website</a>, and is available from the <a href="http://journal.imbio.de/article.php?aid=291">BioBricks Foundation as BBF RFC 112</a>.</span>
</p>