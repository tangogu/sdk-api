---
UID: NF:wmp.IWMPPlaylist.insertItem
title: IWMPPlaylist::insertItem (wmp.h)
description: The insertItem method adds a media item at the specified location in the playlist.
helpviewer_keywords: ["IWMPPlaylist interface [Windows Media Player]","insertItem method","IWMPPlaylist.insertItem","IWMPPlaylist::insertItem","IWMPPlaylistinsertItem","insertItem","insertItem method [Windows Media Player]","insertItem method [Windows Media Player]","IWMPPlaylist interface","wmp.iwmpplaylist_insertitem","wmp/IWMPPlaylist::insertItem"]
old-location: wmp\iwmpplaylist_insertitem.htm
tech.root: WMP
ms.assetid: 2db2d28d-4cbf-423c-824f-e1e212c46f7a
ms.date: 12/05/2018
ms.keywords: IWMPPlaylist interface [Windows Media Player],insertItem method, IWMPPlaylist.insertItem, IWMPPlaylist::insertItem, IWMPPlaylistinsertItem, insertItem, insertItem method [Windows Media Player], insertItem method [Windows Media Player],IWMPPlaylist interface, wmp.iwmpplaylist_insertitem, wmp/IWMPPlaylist::insertItem
req.header: wmp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Media Player 9 Series or later.
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Wmp.dll
req.irql: 
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
f1_keywords:
 - IWMPPlaylist::insertItem
 - wmp/IWMPPlaylist::insertItem
dev_langs:
 - c++
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - wmp.dll
api_name:
 - IWMPPlaylist.insertItem
---

# IWMPPlaylist::insertItem


## -description

The <b>insertItem</b> method adds a media item at the specified location in the playlist.

## -parameters

### -param lIndex [in]

<b>long</b> containing the index at which this method will add the item.

### -param pIWMPMedia [in]

Pointer to an <b>IWMPMedia</b> interface for the inserted item.

## -returns

The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
</table>

## -remarks

All items after the inserted item will have their index numbers increased by one.

Before calling this method, you must have full access to the library. For more information, see <a href="/windows/desktop/WMP/library-access">Library Access</a>.

## -see-also

<a href="/windows/desktop/api/wmp/nn-wmp-iwmpmedia">IWMPMedia Interface</a>



<a href="/windows/desktop/api/wmp/nn-wmp-iwmpplaylist">IWMPPlaylist Interface</a>



<a href="/windows/desktop/api/wmp/nf-wmp-iwmpplaylist-removeitem">IWMPPlaylist::removeItem</a>