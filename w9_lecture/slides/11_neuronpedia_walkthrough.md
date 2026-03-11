# Neuronpedia Walkthrough: Hands-On with Gemma-2-2B

## A. Feature browsing on Gemma-2-2B
1. Go to **neuronpedia.org** → select **Gemma-2-2B** → pick a layer and SAE
2. Search for a concept (e.g., "sports", "legal", "numbers") or browse by category
3. Click a feature → see **top activating texts**, **activation pattern**, and **logit effects**
4. **Hands-on task:** pick a concept you find interesting — is the feature **monosemantic** (one clear meaning) or polysemantic (mixed)?

## B. Attribution graphs on Gemma-2-2B
1. Go to **neuronpedia.org/gemma-2-2b/graph**
2. Type prompt: **"The state containing Dallas has its capital in"**
3. Click **"Generate Graph"** → an interactive circuit appears in seconds
4. What you see:
   - **Nodes** = active features; **edges** = linear effects between them
   - **Size/color** of nodes indicates importance to the final prediction
5. The graph reveals **two-hop reasoning**: Dallas → "Texas" features → "Austin" features, plus shortcut paths going directly Dallas → Austin
6. **Hover/click** any node to see its full Neuronpedia feature dashboard
7. Adjust the **pruning threshold** slider to show more or fewer connections

## C. Steering (brief)
- You can **steer Gemma-2-2B output** by clamping features — amplify or suppress any feature
- This is the generalized version of **"Golden Gate Claude"** — works with any feature you find
- Rate limit: 100 steers/hour
