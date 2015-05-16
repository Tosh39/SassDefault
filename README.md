# Sass-Default
To build readable css


# NamingGuidelines
```html
<article>
<h1>CSS Naming Rule Guidelines</h1>
<p><small> Author: Toshiki Yamamoto<br>Date: 2014/11/21</small></p>
<p>This is about how to name for each classes.</p>
<section>
	<h2>Purpose:</h2>
    <ul>
    	<li>To make class names short as possible.</li>
        <li>To reduce times for naming and coding, or maintenance when alone and also team.</li>
        <li>To let easy to understand what the class stands for.</li>
    </ul>
</section>
<section>
	<h2>Basic Rules</h2>
    <p>Block is one conponent. Block is consisted by 2 kinds of groups, 'Layout', and 'Module'. Layout means how to display and Module means how to style.</p>
    <table>
    	<tr>
        	<th>Kind</th>
            <th>Include</th>
            <th>Prefix</th>
            <th>Rules</th>
        </tr>
        <tr>
        	<th>Blockname</th>
           	<td>Anything which can affect all through this block.</td>
            <td><i>None</i></td>
            <td>Indicate specific roll for this block.</td>
        </tr>
    	<tr>
        	<th>Layout</th>
            <td>
            	<ul>
                	<li>Margin</li>
                    <li>Padding</li>
                    <li>Box-sizing</li>
                    <li>Position</li>
                    <li>Display</li>
                    <li>Top/Left/Right/Bottom</li>
                </ul>
            </td>
            <td>'l-'</td>
            <td>
            	<ul>	
                	<li>Start from 'l-blockname' (layout)</li>
                    <li>Going to be longer when deeper</li>
                </ul>
            </td>
       	</tr>
        <tr>
        	<th>Module</th>
            <td>
            	<ul>
                	<li>Font</li>
                    <li>Color</li>
                    <li>Ackground</li>
                    <li>Line-height</li>
                    <li>Transform</li>
                    <li>Transition</li>
                    <li>and so on.</li>
                </ul>
            </td>
            <td>'c-' or 'g-'</td>
            <td>
            	<ul>
                    <li>This is separated by 3 parts, 'how deep', 'blockname', 'specific name'.</li>
                	<li>How deep is 'c-blockname' (child: 1)<br />or 'g-blockname' (grandchild: 2)</li>
                    <li>Deeper than grand-child, its going to be like; 'cg-' (3), 'ggg-' (6).</li>
                </ul>
           	</td>
        </tr>
    </table>
    <h2>Supported Rules</h2>
    <p>Supported Rules are so important to prevent canceling of each classes.</p>
    <table>
    	<tr>
        	<th>Kind</th>
            <th>Include</th>
            <th>Prefix</th>
            <th>Rules</th>
        </tr>
        <tr>
        	<th>State</th>
            <td>Anything to add or remove when the state changes.</td>
            <td>'is-' or 'has-'</td>
            <td>
            	<ul>
                	<li>This make elements change style by added to or removed from the element.</li>
                    <li>This could use '!important' because this has to affect.</li>
                </ul>
            </td>
        </tr>
        <tr>
        	<th>Utility</th>
            <td>Anything</td>
            <td>'u-'</td>
            <td>Include only ONE or TWO styles</td>
        </tr>
        <tr>
        	<th>Icon</th>
            <td>Only icon related styles</td>
            <td>'ic-'</td>
            <td>This is intended to use with '&lt; span &gt;'</td>
       	</tr>
    </table>
    <h2>Detail Rules</h2>
    <dl>
    	<dt>Independent</dt>
       	<dd>CSS selectors should be only by class, and id in some case.DO NOT use html tags so often.<br />Sometimes, for example 'li' elements with no child element, it can be used.</dd>
        <dt>Capital Letters, NOT Hyphen(-)</dt>
        <dd>If the name is consisted by 2 parts, such as 'side menu', DO NOT use hyphen(-) to make it separate, USE Capital letter.<br />'.sideMenu' is correct.</dd>
    </dl>
</section>
</article>
```
