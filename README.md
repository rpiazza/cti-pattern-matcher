<div>
<h1>README</h1>

<div>
<h2><a id="readme-general">OASIS Open Repository: cti-pattern-matcher</a></h2>

<p>This GitHub public repository ( <b><a href="https://github.com/oasis-open/cti-pattern-matcher">https://github.com/oasis-open/cti-pattern-matcher</a></b> ) was created at the request of the <a href="https://www.oasis-open.org/committees/cti/">OASIS Cyber Threat Intelligence (CTI) TC</a> as an <a href="https://www.oasis-open.org/resources/open-repositories/">OASIS Open Repository</a> to support development of open source resources related to Technical Committee work.</p>

<p>While this Open Repository remains associated with the sponsor TC, its development priorities, leadership, intellectual property terms, participation rules, and other matters of governance are <a href="https://github.com/oasis-open/cti-pattern-matcher/blob/master/CONTRIBUTING.md#governance-distinct-from-oasis-tc-process">separate and distinct</a> from the OASIS TC Process and related policies.</p>

<p>All contributions made to this Open Repository are subject to open source license terms expressed in the <a href="https://www.oasis-open.org/sites/www.oasis-open.org/files/BSD-3-Clause.txt">BSD-3-Clause License</a>.  That license was selected as the declared <a href="https://www.oasis-open.org/resources/open-repositories/licenses">"Applicable License"</a> when the Open Repository was created.</p>

<p>As documented in <a href="https://github.com/oasis-open/cti-pattern-matcher/blob/master/CONTRIBUTING.md#public-participation-invited">"Public Participation Invited</a>", contributions to this OASIS Open Repository are invited from all parties, whether affiliated with OASIS or not.  Participants must have a GitHub account, but no fees or OASIS membership obligations are required.  Participation is expected to be consistent with the <a href="https://www.oasis-open.org/policies-guidelines/open-repositories">OASIS Open Repository Guidelines and Procedures</a>, the open source <a href="https://github.com/oasis-open/cti-pattern-matcher/blob/master/LICENSE">LICENSE</a> designated for this particular repository, and the requirement for an <a href="https://www.oasis-open.org/resources/open-repositories/cla/individual-cla">Individual Contributor License Agreement</a> that governs intellectual property.</p>

</div>

<div>
<h2><a id="purposeStatement">Statement of Purpose</a></h2>

<p>Statement of Purpose for this OASIS Open Repository (cti-pattern-matcher) as <a href="https://lists.oasis-open.org/archives/cti/201610/msg00106.html">proposed</a> and <a href="https://lists.oasis-open.org/archives/cti/201610/msg00126.html">approved</a> [<a href="https://issues.oasis-open.org/browse/TCADMIN-2477">bis</a>] by the TC:</p>

<p>The pattern-matcher is a prototype software tool for matching STIX Observed Data content against patterns used in STIX Indicators. The matcher accepts a pattern and one or more timestamped observations, and determines whether the observations match the criteria specified by the pattern. The purpose of this tool is to evaluate examples and test cases which implement the patterning specification, as a form of executable documentation and to verify patterns express the desired criteria.</p>

<!--  Description: OASIS Open Repository: Match STIX content against STIX patterns -->

</div>


### Requirements
* Python 2.7.6+
* ANTLR Python Runtime (4.5.3+)
  * https://pypi.python.org/pypi/antlr4-python2-runtime (Python 2)
  * https://pypi.python.org/pypi/antlr4-python3-runtime (Python 3)
* python-dateutil (https://dateutil.readthedocs.io/en/stable/)
* six (https://six.readthedocs.io/)
* (For running tests) - pytest (http://pytest.org/latest/getting-started.html)

### Installation

To install pattern-matcher, first install all required dependencies, then run `python setup.py install` in the root of this repository.

### Usage

Run the `pattern_matcher.py` script in this repository, and follow directions. For example:

```bash
$ python pattern_matcher.py

Enter a CybOX pattern:
file-object:hashes.sha-256 = 'aec070645fe53ee3b3763059376134f058cc337247c978add178b6ccdfb0019f'

Enter the name of json file containing a CybOX object or container:
test\0pass.json

PASS: file-object:hashes.sha-256 = 'aec070645fe53ee3b3763059376134f058cc337247c978add178b6ccdfb0019f'
```

### Testing

To run the automated tests, execute `py.test` from inside the `test` directory.


<div>
<h2><a id="maintainers">Maintainers</a></h2>

<p>Open Repository <a href="https://www.oasis-open.org/resources/open-repositories/maintainers-guide">Maintainers</a> are responsible for oversight of this project's community development activities, including evaluation of GitHub <a href="https://github.com/oasis-open/cti-pattern-matcher/blob/master/CONTRIBUTING.md#fork-and-pull-collaboration-model">pull requests</a> and <a href="https://www.oasis-open.org/policies-guidelines/open-repositories#repositoryManagement">preserving</a> open source principles of openness and fairness. Maintainers are recognized and trusted experts who serve to implement community goals and consensus design preferences.</p>

<p>Initially, the associated TC members have designated one or more persons to serve as Maintainer(s); subsequently, participating community members may select additional or substitute Maintainers, per <a href="https://www.oasis-open.org/resources/open-repositories/maintainers-guide#additionalMaintainers">consensus agreements</a>.</p>

<p><b><a id="currentMaintainers">Current Maintainers of this Open Repository</a></b></p>

<ul>
<li><a href="mailto:gback@mitre.org">Greg Back</a>; GitHub ID: <a href="https://github.com/gtback/">https://github.com/gtback/</a>; WWW: <a href="https://www.mitre.org/">MITRE</a></li>
<li><a href="mailto:ikirillov@mitre.org">Ivan Kirillov</a>; GitHub ID: <a href="https://github.com/ikiril01/">https://github.com/ikiril01/</a>; WWW: <a href="https://www.mitre.org/">MITRE</a></li>
</ul>

</div>

<div><h2><a id="aboutOpenRepos">About OASIS Open Repositories</a></h2>

<p><ul>
<li><a href="https://www.oasis-open.org/resources/open-repositories/">Open Repositories: Overview and Resources</a></li>
<li><a href="https://www.oasis-open.org/resources/open-repositories/faq">Frequently Asked Questions</a></li>
<li><a href="https://www.oasis-open.org/resources/open-repositories/licenses">Open Source Licenses</a></li>
<li><a href="https://www.oasis-open.org/resources/open-repositories/cla">Contributor License Agreements (CLAs)</a></li>
<li><a href="https://www.oasis-open.org/resources/open-repositories/maintainers-guide">Maintainers' Guidelines and Agreement</a></li>
</ul></p>

</div>

<div><h2><a id="feedback">Feedback</a></h2>

<p>Questions or comments about this Open Repository's activities should be composed as GitHub issues or comments. If use of an issue/comment is not possible or appropriate, questions may be directed by email to the Maintainer(s) <a href="#currentMaintainers">listed above</a>.  Please send general questions about Open Repository participation to OASIS Staff at <a href="mailto:repository-admin@oasis-open.org">repository-admin@oasis-open.org</a> and any specific CLA-related questions to <a href="mailto:repository-cla@oasis-open.org">repository-cla@oasis-open.org</a>.</p>

</div></div>
