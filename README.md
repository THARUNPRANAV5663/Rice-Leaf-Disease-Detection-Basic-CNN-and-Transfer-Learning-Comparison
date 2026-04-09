
<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: var(--font-sans); }
  .readme { padding: 1.5rem 0; max-width: 860px; }
  .badge { display: inline-block; font-size: 12px; font-weight: 500; padding: 3px 10px; border-radius: 20px; margin-right: 6px; margin-bottom: 4px; }
  .badge-green { background: #EAF3DE; color: #3B6D11; }
  .badge-blue { background: #E6F1FB; color: #185FA5; }
  .badge-purple { background: #EEEDFE; color: #534AB7; }
  .badge-amber { background: #FAEEDA; color: #854F0B; }
  .badge-teal { background: #E1F5EE; color: #0F6E56; }
  .section-title { font-size: 13px; font-weight: 500; color: var(--color-text-secondary); text-transform: uppercase; letter-spacing: 0.08em; margin-bottom: 12px; margin-top: 2rem; }
  .divider { border: none; border-top: 0.5px solid var(--color-border-tertiary); margin: 1.5rem 0; }
  .hero { background: var(--color-background-secondary); border-radius: var(--border-radius-lg); border: 0.5px solid var(--color-border-tertiary); padding: 1.5rem; margin-bottom: 1.5rem; }
  .hero-title { font-size: 22px; font-weight: 500; color: var(--color-text-primary); margin-bottom: 6px; }
  .hero-sub { font-size: 14px; color: var(--color-text-secondary); margin-bottom: 1rem; line-height: 1.6; }
  .metric-grid { display: grid; grid-template-columns: repeat(4, minmax(0, 1fr)); gap: 10px; margin-bottom: 1.5rem; }
  .metric-card { background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-md); padding: 0.75rem 1rem; }
  .metric-label { font-size: 12px; color: var(--color-text-secondary); margin-bottom: 4px; }
  .metric-val { font-size: 20px; font-weight: 500; color: var(--color-text-primary); }
  .metric-val.green { color: #3B6D11; }
  .metric-val.blue { color: #185FA5; }
  .model-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; margin-bottom: 1.5rem; }
  .model-card { background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); padding: 1rem 1.25rem; }
  .model-card.featured { border: 2px solid #378ADD; }
  .model-card-title { font-size: 15px; font-weight: 500; color: var(--color-text-primary); margin-bottom: 4px; }
  .model-card-sub { font-size: 13px; color: var(--color-text-secondary); margin-bottom: 10px; }
  .model-stat { display: flex; justify-content: space-between; font-size: 13px; padding: 4px 0; border-bottom: 0.5px solid var(--color-border-tertiary); }
  .model-stat:last-child { border-bottom: none; }
  .model-stat-label { color: var(--color-text-secondary); }
  .model-stat-val { font-weight: 500; color: var(--color-text-primary); }
  .model-stat-val.good { color: #3B6D11; }
  .model-stat-val.bad { color: #A32D2D; }
  .class-grid { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 10px; margin-bottom: 1.5rem; }
  .class-card { border-radius: var(--border-radius-md); padding: 0.75rem 1rem; border: 0.5px solid var(--color-border-tertiary); }
  .class-card.c1 { background: #E1F5EE; }
  .class-card.c2 { background: #E6F1FB; }
  .class-card.c3 { background: #EEEDFE; }
  .class-name { font-size: 13px; font-weight: 500; margin-bottom: 2px; }
  .class-name.c1 { color: #0F6E56; }
  .class-name.c2 { color: #185FA5; }
  .class-name.c3 { color: #534AB7; }
  .class-count { font-size: 12px; }
  .class-count.c1 { color: #0F6E56; }
  .class-count.c2 { color: #185FA5; }
  .class-count.c3 { color: #534AB7; }
  .setup-steps { list-style: none; }
  .setup-steps li { display: flex; gap: 12px; align-items: flex-start; padding: 8px 0; border-bottom: 0.5px solid var(--color-border-tertiary); font-size: 14px; color: var(--color-text-primary); }
  .setup-steps li:last-child { border-bottom: none; }
  .step-num { min-width: 22px; height: 22px; border-radius: 50%; background: var(--color-background-info); color: var(--color-text-info); font-size: 12px; font-weight: 500; display: flex; align-items: center; justify-content: center; }
  .disclaimer { background: #FAEEDA; border: 0.5px solid #EF9F27; border-radius: var(--border-radius-md); padding: 0.75rem 1rem; font-size: 13px; color: #633806; margin-bottom: 1.5rem; line-height: 1.6; }
  .disclaimer strong { color: #412402; }
  .tech-list { display: flex; flex-wrap: wrap; gap: 6px; margin-bottom: 1.5rem; }
  .notebook-card { background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-md); padding: 0.75rem 1rem; margin-bottom: 8px; display: flex; justify-content: space-between; align-items: center; }
  .notebook-name { font-size: 14px; font-weight: 500; color: var(--color-text-primary); }
  .notebook-desc { font-size: 12px; color: var(--color-text-secondary); margin-top: 2px; }
</style>

<div class="readme">

  <div class="hero">
    <div class="hero-title">Rice Leaf Disease Detection</div>
    <div class="hero-sub">Basic CNN and Transfer Learning Comparison — PRCP-1001 Capstone Project</div>
    <div>
      <span class="badge badge-green">Deep Learning</span>
      <span class="badge badge-blue">Transfer Learning</span>
      <span class="badge badge-purple">MobileNetV2</span>
      <span class="badge badge-amber">Image Classification</span>
      <span class="badge badge-teal">TensorFlow / Keras</span>
    </div>
  </div>

  <div class="metric-grid">
    <div class="metric-card">
      <div class="metric-label">Dataset size</div>
      <div class="metric-val">119</div>
      <div style="font-size:11px;color:var(--color-text-secondary);margin-top:2px;">images total</div>
    </div>
    <div class="metric-card">
      <div class="metric-label">Classes</div>
      <div class="metric-val">3</div>
      <div style="font-size:11px;color:var(--color-text-secondary);margin-top:2px;">disease types</div>
    </div>
    <div class="metric-card">
      <div class="metric-label">Basic CNN accuracy</div>
      <div class="metric-val bad" style="color:#A32D2D;">~48%</div>
      <div style="font-size:11px;color:var(--color-text-secondary);margin-top:2px;">val accuracy</div>
    </div>
    <div class="metric-card">
      <div class="metric-label">Transfer learning accuracy</div>
      <div class="metric-val green">91%</div>
      <div style="font-size:11px;color:var(--color-text-secondary);margin-top:2px;">val accuracy</div>
    </div>
  </div>

  <hr class="divider">
  <div class="section-title">Dataset — classes</div>

  <div class="class-grid">
    <div class="class-card c1">
      <div class="class-name c1">Bacterial leaf blight</div>
      <div class="class-count c1">40 images</div>
    </div>
    <div class="class-card c2">
      <div class="class-name c2">Brown spot</div>
      <div class="class-count c2">40 images</div>
    </div>
    <div class="class-card c3">
      <div class="class-name c3">Leaf smut</div>
      <div class="class-count c3">40 images</div>
    </div>
  </div>

  <div class="disclaimer">
    <strong>Dataset notice:</strong> The dataset is not included in this repository. Download link and instructions are provided in the project Word document (<code>PRCP-1001-RiceLeaf.docx</code>). Direct download: <code>https://d3ilbtxij3aepc.cloudfront.net/projects/CDS-Capstone-Projects/PRCP-1001-RiceLeaf.zip</code>
  </div>

  <hr class="divider">
  <div class="section-title">Model comparison</div>

  <div class="model-grid">
    <div class="model-card">
      <div class="model-card-title">Basic CNN</div>
      <div class="model-card-sub">Sequential model from scratch</div>
      <div class="model-stat"><span class="model-stat-label">Val accuracy</span><span class="model-stat-val bad">~48%</span></div>
      <div class="model-stat"><span class="model-stat-label">Approach</span><span class="model-stat-val">Random init weights</span></div>
      <div class="model-stat"><span class="model-stat-label">Issue</span><span class="model-stat-val bad">Overfitting</span></div>
      <div class="model-stat"><span class="model-stat-label">Augmentation</span><span class="model-stat-val">None</span></div>
    </div>
    <div class="model-card featured">
      <div style="margin-bottom:8px;"><span class="badge badge-blue">Recommended</span></div>
      <div class="model-card-title">MobileNetV2</div>
      <div class="model-card-sub">Transfer learning — feature extraction</div>
      <div class="model-stat"><span class="model-stat-label">Val accuracy</span><span class="model-stat-val good">91%</span></div>
      <div class="model-stat"><span class="model-stat-label">Approach</span><span class="model-stat-val">ImageNet pretrained</span></div>
      <div class="model-stat"><span class="model-stat-label">Trainable params</span><span class="model-stat-val">164K / 2.4M</span></div>
      <div class="model-stat"><span class="model-stat-label">Augmentation</span><span class="model-stat-val good">Yes</span></div>
    </div>
  </div>

  <hr class="divider">
  <div class="section-title">Setup instructions</div>

  <ul class="setup-steps">
    <li><span class="step-num">1</span>Download the dataset from the link in the Word document</li>
    <li><span class="step-num">2</span>Extract the zip and upload to Google Drive</li>
    <li><span class="step-num">3</span>Create a folder called <code>Data</code> inside <code>MyDrive</code></li>
    <li><span class="step-num">4</span>Place the 3 class folders inside <code>Data/</code></li>
    <li><span class="step-num">5</span>Open notebook in Google Colab and run <code>drive.mount()</code> cell first</li>
  </ul>

  <hr class="divider">
  <div class="section-title">Notebooks</div>

  <div class="notebook-card">
    <div>
      <div class="notebook-name">PRCP_1001_RiceLeaf_Basic.ipynb</div>
      <div class="notebook-desc">Sequential CNN from scratch — EDA, preprocessing, model training, evaluation</div>
    </div>
    <span class="badge badge-amber">Basic</span>
  </div>
  <div class="notebook-card">
    <div>
      <div class="notebook-name">PRCP_1001_RiceLeaf_Advanced.ipynb</div>
      <div class="notebook-desc">MobileNetV2 transfer learning — ImageDataGenerator, EarlyStopping, ModelCheckpoint, ReduceLROnPlateau</div>
    </div>
    <span class="badge badge-blue">Advanced</span>
  </div>

  <hr class="divider">
  <div class="section-title">Tech stack</div>
  <div class="tech-list">
    <span class="badge badge-blue">Python</span>
    <span class="badge badge-blue">TensorFlow / Keras</span>
    <span class="badge badge-purple">MobileNetV2</span>
    <span class="badge badge-green">NumPy</span>
    <span class="badge badge-green">Matplotlib</span>
    <span class="badge badge-green">Seaborn</span>
    <span class="badge badge-teal">scikit-learn</span>
    <span class="badge badge-amber">Google Colab</span>
  </div>

</div>
