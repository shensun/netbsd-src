#	$NetBSD: Makefile,v 1.9 2008/08/05 20:57:45 pooka Exp $
#	@(#)Makefile	8.2 (Berkeley) 3/27/94

.include <bsd.own.mk>

PROG=	mount_lfs
SRCS=	mount_lfs.c pathadj.c
MAN=	mount_lfs.8

MOUNT=	${NETBSDSRCDIR}/sbin/mount
CPPFLAGS+=-I${MOUNT} -DWANT_CLEANER
.PATH:	${MOUNT}

DPADD+=${LIBUTIL}
LDADD+=-lutil

.include <bsd.prog.mk>
