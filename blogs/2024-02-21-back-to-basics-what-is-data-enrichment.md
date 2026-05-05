---
title: "Back to basics: What is data enrichment?"
url: "https://www.basiq.io/blog/back-to-basics-what-is-data-enrichment/"
date: "Wed, 21 Feb 2024 01:03:04 +0000"
author: "Alex McManus"
feed_url: "https://www.basiq.io/blog/feed/"
---
<p>Looking at your banking app, what was the last purchase you made? Depending on your bank, you might see the:</p>



<ul class="wp-block-list">
<li>merchant name (maybe even their logo?)&nbsp;</li>



<li>amount spent&nbsp;</li>



<li>time of purchase</li>



<li>geographic location&nbsp;</li>
</ul>



<p>What you don’t see is the refinement process the transaction data goes through before it’s displayed. This is called data enrichment. It takes the messy raw transaction data and turns it into clean descriptions by adding the merchant&#8217;s identity, location and categorisation details (as seen below).&nbsp;</p>



<figure class="wp-block-image size-large"><img alt="" class="wp-image-16359" height="535" src="https://wordpress.basiq.io/blog/wp-content//uploads/2024/02/enrich_07-1024x535.png" width="1024" /></figure>



<p>Let’s go behind the scenes and explore how we turn data into insights using <a href="https://www.basiq.io/products/enrich/">Basiq Enrich</a>.&nbsp;</p>



<h2 class="wp-block-heading"><strong>The data enrichment process</strong></h2>



<p>Enriching banking data via the Basiq platform is a four-step process:&nbsp;</p>



<ol class="wp-block-list">
<li>Data access</li>



<li>Data tagging, cleaning and tokenisation</li>



<li>Data enrichment</li>



<li>Machine Learning and final output</li>
</ol>



<p>Let’s go over each in more detail.&nbsp;</p>



<h2 class="wp-block-heading">Step 1: Data access&nbsp;</h2>



<p>The first step is accessing a customer’s transaction data. To do this, customers consent to securely link their bank accounts using <a href="https://www.basiq.io/products/connect/">Basiq Connect</a>.&nbsp;</p>


<div class="wp-block-image">
<figure class="aligncenter size-full"><img alt="" class="wp-image-16360" height="480" src="https://wordpress.basiq.io/blog/wp-content//uploads/2024/02/Connect.png" width="601" /></figure>
</div>


<h2 class="wp-block-heading">Step 2: Tag, clean and tokenise</h2>



<p>Once the raw banking data is collected from a user’s account, transactions are separated into debits or credits</p>



<figure class="wp-block-table"><table><tbody><tr><td><strong>Debit</strong></td><td><strong>Credit</strong></td></tr><tr><td><strong>Bank fee</strong><br />A fee incurred by the user from their bank e.g. ATM withdrawal fee<br /><br /><strong>Payment</strong>Payment made to a merchant&nbsp;<br /><strong>Cash withdrawal</strong>&nbsp;Funds withdrawn via an ATM<br /><strong>Transfer</strong>&nbsp;&nbsp;Funds transferred to an account&nbsp;<br /><strong>Loan interest&nbsp;</strong>Interest charged on a loan account&nbsp;</td><td><strong>Refund</strong>Funds returned to account due to refund<br /><strong>Interest</strong>Interest earned<br /><strong>Transfer&nbsp;</strong>Funds received from an account&nbsp;<br /><strong>Loan repayment</strong>Loan repayment credited to a loan account&nbsp;</td></tr></tbody></table></figure>



<p>Once transactions are identified, the Basiq platform uses the transaction metadata to clean and standardise the data ready for enrichment. Below is an example of this process using a purchase from energy provider, Momentum Energy.</p>



<figure class="wp-block-image size-large"><img alt="" class="wp-image-16361" height="111" src="https://wordpress.basiq.io/blog/wp-content//uploads/2024/02/enrich_02-1024x111.png" width="1024" /></figure>



<figure class="wp-block-image size-large"><img alt="" class="wp-image-16362" height="282" src="https://wordpress.basiq.io/blog/wp-content//uploads/2024/02/enrich_03-1024x282.png" width="1024" /></figure>



<p>Unfortunately, there is no consistent format for transaction data across banks, so standardisation is a crucial step. For example, the image below illustrates how a transaction with footwear retailer, Tony Bianco, is returned from four different banks. To meet this challenge Basiq maintains a database of transaction description patterns by bank so enrichment can be customised depending on the institution.&nbsp;</p>



<figure class="wp-block-image size-large"><img alt="" class="wp-image-16363" height="282" src="https://wordpress.basiq.io/blog/wp-content//uploads/2024/02/enrich_01-1024x282.png" width="1024" /></figure>



<h2 class="wp-block-heading">Step 3: Data enrichment&nbsp;&nbsp;</h2>



<p>Once tagged, cleaned and tokenised, the Basiq platform enriches the payment data by searching for a match in our curated merchant database which includes the identity, location and categorisation details.</p>



<figure class="wp-block-image size-large"><img alt="" class="wp-image-16364" height="282" src="https://wordpress.basiq.io/blog/wp-content//uploads/2024/02/enrich_04-1024x282.png" width="1024" /></figure>



<p>When it comes to categorisation, we provide five levels of categorisation enabling greater granularity and richer insights. This includes four levels of <a href="https://www.dcceew.gov.au/environment/protection/npi/reporting/industry-reporting-materials/anzsic-code-list">ANZSIC categorisation</a> (‘Division’, ‘Sub Division’, ‘Group’ and ‘Class’) and an additional ‘Sub Class’ using Basiq’s unique categorisation database.</p>



<h2 class="wp-block-heading">Step 4: Machine Learning and final output</h2>



<p>In our enrichment process, when a transaction cannot be initially categorised and enriched, our advanced machine learning model intervenes. This model leverages additional data sources, meticulously analysing transactions to fill any gaps that might remain after the initial steps.<br /><br />Our goal with this approach is to ensure near-perfect accuracy in the data output. What sets it apart is its dynamic learning capability. With each transaction it processes, the ML model evolves improving its efficiency and accuracy.&nbsp;<br />After the data has been enriched the process is complete and it’s ready for output – like your banking app.&nbsp;</p>



<figure class="wp-block-image size-large"><img alt="" class="wp-image-16365" height="178" src="https://wordpress.basiq.io/blog/wp-content//uploads/2024/02/enrich_05-1024x178.png" width="1024" /></figure>



<figure class="wp-block-image size-large"><img alt="" class="wp-image-16366" height="383" src="https://wordpress.basiq.io/blog/wp-content//uploads/2024/02/enrich_06-1024x383.png" width="1024" /></figure>



<p>Basiq Enrich transforms transaction data from banking apps into clear insights.<br />How? By securely accessing transaction data (with permission) and applying magic—tagging, cleaning, and enrichment across each transaction using our vast merchant database and advanced machine learning.<br /><br />Our goal? To make your financial data easy to understand and insightful. With Basiq Enrich, you don&#8217;t just see numbers and codes; you see your spending story unfold. It&#8217;s all about clarity, insight, and helping you make sense of where your money goes, making your banking experience not just informative but genuinely enlightening.</p>



<h2 class="wp-block-heading" id="want-to-know-more">Want to know more?</h2>



<p>Check out how Basiq customers are using Enrich; <a href="https://www.basiq.io/blog/empowering-community-sports-through-clubfunders-innovative-sponsorship-payment-solutions/">Clubfunders</a>, <a href="https://www.basiq.io/blog/from-super-funds-to-charities-pokitpals-new-round-up-solution-empowers-users-with-open-banking/">PokitPal</a> and <a href="https://www.basiq.io/blog/taxtank-is-empowering-customers-to-manage-their-tax-in-real-time-with-open-banking/">TaxTank</a>. </p>



<p>Or <a href="https://www.basiq.io/contact/">get in touch</a> with the Basiq team to find out more.</p>



<div class="accordion accordion--simple js-scroll-animation" id="accordion">
	<div class="accordion-item">
		<div class="accordion-title">
			<h5>
				Article Sources			</h5>
		</div><!-- /.accordion-title -->

		<div class="accordion-header" id="accordion-heading-article-sources69f7d8facf040">
			<button class="accordion-button collapsed" type="button">
				<strong>
					Article Sources				</strong>

				<strong>
					<span>
						Read more					</span>

					<span>
						Read less					</span>
				</strong>
			</button>
		</div><!-- /.accordion-header -->

		<div class="accordion-collapse collapse" id="accordion-article-sources69f7d8facf040">
			<p>Basiq mandates its writers to leverage primary sources such as internal data, industry research, white papers, and government data for their content. They also consult with industry professionals for added insights. Rigorous research, review, and fact-checking processes are employed to uphold accuracy and ethical standards, while valuing reader engagement and adopting inclusive language. Continuous updates are made to reflect current financial technology trends. You can delve into the principles we adhere to for ensuring reliable, actionable content in our <a href="http://docs.basiq.io/en/articles/8461896-basiq-s-editorial-policy" rel="noopener" target="_blank">editorial policy</a>.</p>
		</div><!-- /.accordion-collapse -->
	</div><!-- /.accordion-item -->
</div><!-- /.accordion -->
<p>The post <a href="https://www.basiq.io/blog/back-to-basics-what-is-data-enrichment/">Back to basics: What is data enrichment?</a> appeared first on <a href="https://www.basiq.io/blog">Open Banking API Platform - Basiq</a>.</p>
